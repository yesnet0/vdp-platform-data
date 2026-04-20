# vdp-platform-data

Structured, machine-readable data for public **VDPs and bug bounty programs** hosted on major coordination platforms.

Inspired by and complementary to [`arkadiyt/bounty-targets-data`](https://github.com/arkadiyt/bounty-targets-data), this repository differs in two ways:

1. **Scope includes no-bounty VDPs**, not just bounty-paying programs.
2. **Platform-hosted only** — programs directly hosted on HackerOne, Bugcrowd, Intigriti, etc. Community-managed lists are excluded.

## Repository layout

```
data/
  hackerone/   # per-platform JSON artifacts
  bugcrowd/
  intigriti/
schema/
  program.schema.json   # canonical program record schema
```

## Not in this repository

This repo holds **data only**. The scraper that produces these artifacts lives in a separate repository (internal). Pull requests that add code to this repo will be declined — open issues against the scraper instead.

## Status

Scaffolding only. No data artifacts have been published yet.

## Licence

See `LICENSE`.
