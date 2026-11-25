# stat-snapshot-data

Public archive of official statistics for Portugal, as published, every night.
It is built by **Stat snapshot** (singledev.eu), a small service that fetches a set of
indicators once a day, keeps every version of every value, and flags **silent revisions**:
past values that change after publication, or that are recalculated with a new method.

Archived since **2026-11-20**. Revisions published before that date cannot be seen here:
the first stored value of each period is the value as it stood on the first fetch.

## What is in this repo
- `data/<series-id>.csv`: the full version history of each series, one CSV per series,
  committed every night. The git history of this repo is the public, timestamped timeline.
- The website at <https://stats.singledev.eu> (GitHub Pages, served from `main`): revision
  tables, vintage charts, methodology-change notices, CSV downloads and the SHA-256 of every
  stored raw payload, so the archive can be checked against the sources.

## Sources and licences
The data belongs to its publishers. This repo republishes it unchanged, with attribution:
- **Eurostat** (European Commission). Reuse is allowed under the
  [Eurostat copyright and reuse policy](https://ec.europa.eu/eurostat/about-us/policies/copyright)
  (Commission Decision 2011/833/EU; CC BY 4.0). Source: Eurostat.
- **INE, Statistics Portugal** (Instituto Nacional de Estatística). Licensed under
  [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Source: INE.
- **Banco de Portugal** (BPstat). Reused under the
  [Banco de Portugal terms of use](https://bpstat.bportugal.pt/). Source: Banco de Portugal.

Stat snapshot is not affiliated with or endorsed by any of these institutions. Values are
copied as published; any errors in processing are ours, not theirs.
