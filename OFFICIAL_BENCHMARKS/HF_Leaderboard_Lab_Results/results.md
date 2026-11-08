# HF_Leaderboard_Lab_Results

**Project:** `K_HEXSTRIKE`  
**Tier:** `TIER_6_SECURITY_EVAL`  
**Slug:** `0x4m4/hexstrike-ai`  
**Commit:** `d689933ff579`  
**Run:** `2026-09-30T15:07:07.146295+00:00`  

## Isolation Environment

| Field | Value |
| ----- | ----- |
| Platform | `win32` |
| Python | `3.12.10` |
| HF model | `distilbert-base-uncased` |
| HF load time | `4.42s` |
| Inference device | `cpu` |

## Results

**Framework:** [HuggingFace Open LLM Leaderboard (proxy via distilbert-base-uncased)](https://huggingface.co/docs/leaderboards/en/open_llm_leaderboard/archive)

**Model used:** `distilbert-base-uncased`

### Inference Latency (Classification)

| Metric | Value |
| ------ | ----- |
| Avg latency | **40.69 ms** |
| Min latency | 34.53 ms |
| Max latency | 47.05 ms |
| Samples | 5 |

### Real Tokenization Results

| Field | Value |
| ----- | ----- |
| Token count | **44** |
| Tokenization latency | 0.0 ms |
| Classification label | `LABEL_0` |
| Classification score | 0.591 |
| Classification latency | 84.99 ms |
| Status | **PASS** |

**Input text tokenized:**
```
K_HEXSTRIKE (0x4m4/hexstrike-ai) — 14 files, 14297 source lines, licence MIT, primary language ['Python']
```

**First 20 tokens:**
```
['[CLS]', 'k', '_', 'he', '##x', '##st', '##rik', '##e', '(', '0', '##x', '##4', '##m', '##4', '/', 'he', '##x', '##st', '##rik', '##e']
```

> Full MMLU/HellaSwag/TruthfulQA/ARC/Winogrande/GSM8K require dedicated GPU.
> These results are CPU inference proxy metrics using distilbert-base-uncased.

---
_Anticloud Benchmark Suite — isolation log — 2026-09-30T15:07:07.146295+00:00_