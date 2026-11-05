# Contributing / 贡献指南

Thank you for helping keep this list accurate.

## Rules
1. **No fabricated entries.** Every paper needs a real arXiv / DOI / publisher URL; every project needs a real homepage or GitHub URL.
2. Prefer entries with code or datasets when available.
3. Keep the bilingual section headers (`中文 / English`).
4. One-line notes should stay factual (method/domain), not marketing claims.
5. Earth / hydrology applications (underwater, construction, disaster, monitoring) are especially welcome.

## Format
```
- **Title** — Authors (Year) [[arXiv](https://arxiv.org/abs/XXXX.XXXXX)] [[Code](https://...)] *(venue)* — _short note_
```

## Process
1. Open a PR against `main`.
2. Optionally add a matching object to `data/papers.json`.
3. Automated 3-day refresh may merge incremental verified finds; duplicates will be deduped by arXiv id / URL.
