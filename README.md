[![make.fun · site-generator-speed-01-run-20261122](https://make.fun/badge/site-generator-speed-01-run-20261122.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![rank](https://make.fun/badge/site-generator-speed-01-run-20261122/TheNumbers-sys/makefun-site-generator-speed-01-run-20261122/rank.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![reward](https://make.fun/badge/site-generator-speed-01-run-20261122/TheNumbers-sys/makefun-site-generator-speed-01-run-20261122/reward.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)

# makefun-site-fast

A faster drop-in for make.fun's own makefun-site 1.0.0: `solve.js` answers
exactly as makefun-site 1.0.0 does for every case — the same output tree
(each page's `index.html`, the index and tag pages, `build-report.txt`, each
static file), byte for byte — but faster. Written from scratch in dependency-free
JavaScript: a single-pass Markdown renderer with index-based inline scanning, a
memoised slugifier, a hand-rolled front-matter parser, and templates compiled
to plain functions (with a tree-walking interpreter as fallback).

`main.ts` is the house driver: it reads every case from
`/input/cases.json`, answers each with `run()` from `solve.js`, and writes
`/output/answers.json`.
