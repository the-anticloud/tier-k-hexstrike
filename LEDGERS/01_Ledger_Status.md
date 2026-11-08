# Ledger Status

**Project:** `K_HEXSTRIKE`  
**Tier:** TIER_6_SECURITY_EVAL  
**Identity:** Upstream `0x4m4/hexstrike-ai` @ `d689933ff579` (MIT)

## Chain state

| Fact | Value |
| --- | --- |
| Upstream | `0x4m4/hexstrike-ai` |
| Commit | `d689933ff579d839c676c82b231f8e98326c5f04` |
| Upstream licence | MIT |
| Licence class | permissive |
| Clone size | 2.8 MB |
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
