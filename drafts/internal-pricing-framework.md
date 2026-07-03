# Internal Pricing Framework

This document captures the current working pricing logic for the website voice agent.

It is an internal working document, not approved public copy.

## Purpose

The agent needs a pricing framework it can reason with without:

- inventing numbers
- creating pricing cliffs
- underpricing enterprise usage
- exposing internal pricing logic too casually

## Current Working Model

### Annual program

- `Growth`: `EUR 24,000` for `50-150` employees
- `Expansion`: `EUR 32,000` for `150-250` employees
- `Scale`: `EUR 40,000` for `250-500` employees
- `Enterprise`: `500+` employees using the balanced degressive model below

### Pilot

- `EUR 50 per person`
- one wave only
- small subset only
- lighter output than the full annual program
- designed as a low-risk trust buy-in

The pilot exists to let a buyer test the experience, build confidence, and decide whether broader rollout is justified.

The pilot should not be presented as equivalent to the annual program.

The intended commercial logic is:

- if they like it, they roll it out
- if they do not, they have lost very little

## Enterprise Pricing Logic

The current preferred model is:

- anchor at `EUR 40,000` through `500`
- then add a degressive per-employee charge above `500`

### Balanced enterprise model

- `501-1,000`: `EUR 35` per employee above `500`
- `1,001-2,000`: `EUR 28` per employee above `1,000`
- `2,001+`: `EUR 22` per employee above `2,000`

### Formula

```text
if employees <= 500:
  annual_price = band_price

if 501 <= employees <= 1000:
  annual_price = 40000 + ((employees - 500) * 35)

if 1001 <= employees <= 2000:
  annual_price = 40000 + (500 * 35) + ((employees - 1000) * 28)

if employees >= 2001:
  annual_price = 40000 + (500 * 35) + (1000 * 28) + ((employees - 2000) * 22)
```

### Example outputs

- `500`: `EUR 40,000`
- `600`: `EUR 43,500`
- `750`: `EUR 48,750`
- `1,000`: `EUR 57,500`
- `1,500`: `EUR 71,500`
- `2,500`: `EUR 96,500`

## Why This Model

This model tries to balance:

- no sudden pricing shock at `501`
- enough revenue protection for token-heavy delivery
- support for full-participant inclusion
- a cleaner story than one-off custom pricing from the first enterprise step
- a clear trust-building entry path through the pilot

## Cost Logic Behind It

This model assumes the delivery cost is not trivial because:

- transcripts are processed more than once
- there is voice-model cost
- there is verification cost
- there is downstream synthesis and reporting cost
- the annual program runs twice yearly

That means enterprise pricing should be degressive, but not aggressively discounted.

## Public-Safe Version

The bot should not automatically expose the full internal calculation.

Public-safe version:

- share fixed bands up to `500`
- say enterprise pricing starts above `Scale` and is based on participation volume and delivery complexity
- offer a tailored estimate once the company size is known

## Inputs The Agent Needs

To use this pricing model well, the agent should gather:

- company name
- role
- approximate employee count
- whether the conversation is about pilot or annual program
- likely participant scope
- whether there are complexity factors such as:
  - multiple geographies
  - multiple business units
  - multiple languages
  - unusual reporting needs

## Recommended Agent Output Structure

The agent should convert the conversation into a structured pricing object before rendering any chart or summary.

Example:

```json
{
  "company_name": "ExampleCo",
  "role": "CEO",
  "employee_count": 780,
  "program_type": "annual",
  "tier": "Enterprise",
  "base_price_eur": 40000,
  "incremental_price_eur": 9800,
  "estimated_annual_price_eur": 49800,
  "calculation_model": "balanced-enterprise-v1",
  "public_safe": true
}
```

## Visual Output Use

If the front end supports live presentation cards, this pricing object can feed:

- pricing summary cards
- tier comparison tables
- enterprise estimate charts
- pilot vs annual comparison views

The agent should not promise a rendered chart unless the front end actually supports it.
