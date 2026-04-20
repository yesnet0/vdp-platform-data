# vdp-platform-data

**Schema and future-home** for machine-readable data on public **VDPs and bug bounty programs** hosted on major coordination platforms.

Inspired by and complementary to [`arkadiyt/bounty-targets-data`](https://github.com/arkadiyt/bounty-targets-data), with two differences:

1. **Scope includes no-bounty VDPs**, not just bounty-paying programs.
2. **Platform-hosted only** — programs directly hosted on HackerOne, Bugcrowd, Intigriti, YesWeHack, etc. Community-managed lists are excluded.

## Where the data lives today

Produced by the scraper at [`yesnet0/platform-scraper`](https://github.com/yesnet0/platform-scraper) and published as **workflow artifacts** on a weekly run:

> https://github.com/yesnet0/platform-scraper/actions

Each run uploads a `bug-bounty-programs-<run_id>` artifact (30-day retention) containing a single `programs-YYYY-MM-DD.json` file conforming to the schema in this repo.

Committed JSON snapshots inside this repo may be added later; for now, artifacts are the canonical distribution.

## Repository layout

```
schema/
  program.schema.json   # canonical program record schema
data/
  hackerone/            # reserved per-platform dirs for future committed snapshots
  bugcrowd/
  intigriti/
  yeswehack/
```

## Scope

This repository holds **schema and (eventually) data** only. Issues about data content, scraper coverage, or platform access should be opened against [`platform-scraper`](https://github.com/yesnet0/platform-scraper). Pull requests that add code here will be declined.

## Licence

[CC0 1.0 Universal](./LICENSE) — public domain dedication.
