# Deposit instructions — team_28, Tier 3, `secondary-2` (deadline: TODAY, Aug 31, end of day)

This repository is **complete and validated** (`make check`: PASS, 43/0/0). Nothing needs to be
edited. What remains is only the release-and-email mechanics below.

## This entry, at a glance

| | |
|---|---|
| Entry | `secondary-2` (team primary is the Tier-1 entry `team28-t1-primary-qwen-nothink`) |
| Approach | Claude Opus 5, direct ATE forecast, literature-conditioned prompt, median of 5 runs |
| Prediction file | `predictions/team_28_T3_secondary-2_v1.csv` (208 ATEs = 16 interventions × 13 outcomes) |
| SHA-256 | `ae461917e1643981f7f4782953a803550a72b621b946f687978d8a7426b482f8` |
| Registration | `registration.md` — fully filled, incl. blinding attestation and exposure disclosure (I.3/I.4) |
| Zenodo metadata | `.zenodo.json` — generated, committed; do not hand-edit |

## Steps to deposit (in this order)

1. **Zenodo toggle — repo owner (Jing) only, BEFORE the release**:
   zenodo.org → Log in with GitHub → account menu → *GitHub* → *Sync now* →
   switch **ON** for `lieblingszz/team28-tier3-secondary-2`.
2. **Publish a GitHub release**: repo → *Releases* → *Create a new release* →
   tag `v1.0` → *Publish release*. Zenodo archives it automatically.
3. **Collect the DOI**: appears on the Zenodo GitHub page a few minutes after the release
   (prefer the concept DOI, "Cite all versions").
4. **One email for the whole team** (reply to Jan Pfänder's reminder thread,
   janlukas.pfaender@gmail.com), containing:
   - **all** the team's deposit DOIs (this entry + Tier-1 primary + secondary-1 + any others);
   - the SHA-256 fingerprint of each prediction file — this entry's line to paste:
     `team_28_T3_secondary-2_v1.csv  sha256: ae461917e1643981f7f4782953a803550a72b621b946f687978d8a7426b482f8`
   - which entry is the team's **primary** (the Tier-1 entry);
   - the **signed exposure declaration** (one per team, one member signs for everyone;
     it is a "yes": Max Pellert attended a 5-minute preliminary-results talk at the
     Behavioral Clones workshop, MPI Berlin, May 2026 — already confirmed with the
     organizers on 20 Aug 2026 and disclosed in `registration.md` I.3/I.4).

## Reminders for the OTHER team repos (from the organizers' last email)

- Any repo copied from another one must re-run `make manifest` and `make zenodo_citation`
  before releasing, otherwise stale files/fingerprints ship in the permanent record.
  In particular, `team28-tier3-secondary-1`'s `metadata.json` had an **empty `sha256`**
  and **empty ORCIDs** as of Aug 30 — fix before releasing.
- Run `make check` in every repo before its release.
- Every entry's registration must carry the same corrected I.3/I.4 exposure disclosure.
