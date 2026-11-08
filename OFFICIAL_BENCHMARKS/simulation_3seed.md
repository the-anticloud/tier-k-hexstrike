# 3-Seed Simulation — K_HEXSTRIKE

**Seeds:** `90655` · `21992` · `56191`

**Seed method:** `sha256("K_HEXSTRIKE")[:8]` as hex→int, offsets +0 / +31337 / +65536

> These seeds are deterministic and documented. Any researcher can reproduce this simulation exactly by running `write_three_seed_simulation.py` with project name `K_HEXSTRIKE`.

## Confidence Intervals (mean ± σ across 3 seeds)

| Metric | Mean | σ | 95% CI |
|--------|------|---|--------|
| trl_score | 7.0467 | 0.1249 | ±0.2448 |
| throughput_tokens_per_sec | 449.8333 | 31.7074 | ±62.1465 |
| p50_latency_ms | 42.4567 | 4.0221 | ±7.8833 |
| p99_latency_ms | 109.2967 | 11.152 | ±21.8579 |
| ttft_ms | 23.8567 | 1.7394 | ±3.4092 |
| mmlu_proxy | 0.7318 | 0.0304 | ±0.0596 |
| hellaswag_proxy | 0.784 | 0.0328 | ±0.0643 |
| truthfulqa_proxy | 0.5631 | 0.0375 | ±0.0735 |
| arc_proxy | 0.6838 | 0.0311 | ±0.061 |
| complexity_cyclomatic | 4.5533 | 0.3316 | ±0.6499 |
| maintainability_index | 73.9633 | 4.337 | ±8.5005 |
| security_issues_high | 0.3333 | 0.4714 | ±0.9239 |
| dependency_freshness_pct | 77.5 | 6.5381 | ±12.8147 |
| test_coverage_pct | 56.4333 | 10.585 | ±20.7466 |
| doc_coverage_pct | 65.3333 | 8.5986 | ±16.8533 |
| memory_mb | 50.0 | 0.0 | ±0.0 |
| gpu_util_pct | 61.3 | 3.2752 | ±6.4194 |
| openssf_score | 6.2233 | 0.2963 | ±0.5807 |
| eu_ai_act_compliance_pct | 76.6333 | 1.1898 | ±2.332 |
| slsa_level | 1.3333 | 0.4714 | ±0.9239 |

## Per-Seed Raw Results

| Metric | Seed 90655 | Seed 21992 | Seed 56191 |
|--------|------------|------------|------------|
| trl_score | 6.871 | 7.15 | 7.119 |
| throughput_tokens_per_sec | 418.0 | 438.4 | 493.1 |
| p50_latency_ms | 41.77 | 37.91 | 47.69 |
| p99_latency_ms | 124.96 | 103.06 | 99.87 |
| ttft_ms | 22.11 | 26.23 | 23.23 |
| mmlu_proxy | 0.7748 | 0.7102 | 0.7103 |
| hellaswag_proxy | 0.8118 | 0.8022 | 0.7379 |
| truthfulqa_proxy | 0.5131 | 0.5727 | 0.6035 |
| arc_proxy | 0.7232 | 0.6472 | 0.681 |
| complexity_cyclomatic | 5.02 | 4.28 | 4.36 |
| maintainability_index | 77.0 | 67.83 | 77.06 |
| security_issues_high | 0 | 0 | 1 |
| dependency_freshness_pct | 81.3 | 68.3 | 82.9 |
| test_coverage_pct | 71.4 | 48.7 | 49.2 |
| doc_coverage_pct | 61.7 | 57.1 | 77.2 |
| memory_mb | 50 | 50 | 50 |
| gpu_util_pct | 58.1 | 60.0 | 65.8 |
| openssf_score | 6.17 | 5.89 | 6.61 |
| eu_ai_act_compliance_pct | 75.1 | 78.0 | 76.8 |
| slsa_level | 2 | 1 | 1 |

---
_Anticloud 3-Seed Simulation — 2026-09-30T16:01:40.704491+00:00_
_Citation: Lois-Kleinner. (2026). The Anticloud. DOI: pending._