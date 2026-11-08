# Ledger Status

**Project:** `L_OPENCOMP`  
**Tier:** TIER_6_SECURITY_EVAL  
**Identity:** Upstream `open-compass/opencompass` @ `e2d2b9a5236b` (Apache-2.0)

## Chain state

| Fact | Value |
| --- | --- |
| Upstream | `open-compass/opencompass` |
| Commit | `e2d2b9a5236ba6a2f0a855af93796e4489c268b7` |
| Upstream licence | Apache-2.0 |
| Licence class | permissive |
| Clone size | 12.9 MB |
| Ledger | 0 blocks, chain verified |
| Current TRL | NOT YET MEASURED |
| Post-optimisation TRL | NOT YET MEASURED |
| II budget cap | 1500.0 IIU |
| Verified upstream edits | 1 |

- Blocks: **0**
- Head digest: `None`
- Chain verification: **verified**

## Independent verification

The chain is verifiable without trusting this project's tooling:

```
anticloud ledger verify
anticloud ledger export > ledger.jsonl
```

Each block carries the previous block's digest, so removing or reordering an
entry invalidates every block after it. That property is the reason the
ledger can stand in for a claim of what happened.
