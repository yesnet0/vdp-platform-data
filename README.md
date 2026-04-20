# vdp-platform-data

Structured, machine-readable data for public **VDPs and bug bounty programs** hosted on major coordination platforms.

Inspired by and complementary to [`arkadiyt/bounty-targets-data`](https://github.com/arkadiyt/bounty-targets-data), this repository differs in two ways:

1. **Scope includes no-bounty VDPs**, not just bounty-paying programs.
2. **Platform-hosted only** — programs directly hosted on HackerOne, Bugcrowd, Intigriti, YesWeHack, etc. Community-managed lists are excluded.

## Repository layout

```
data/
  hackerone/   # per-platform JSON artifacts
  bugcrowd/
  intigriti/
  yeswehack/
schema/
  program.schema.json   # canonical program record schema
```

## Source

The scraper that produces these artifacts lives at [`yesnet0/platform-scraper`](https://github.com/yesnet0/platform-scraper). It fetches every platform directly from its own canonical public endpoint — no community aggregator is used as an authoritative source.

Issues about data content, coverage, or scraper behaviour should be opened against `platform-scraper`. This repository holds **data only** — pull requests that add code here will be declined.

## Status

Scaffolding. Data artifacts will be published by the scraper's weekly GitHub Actions run.

## Licence

[CC0 1.0 Universal](./LICENSE) — public domain dedication.
