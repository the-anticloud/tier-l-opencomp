# HF_Leaderboard_Lab_Results

**Project:** `L_OPENCOMP`  
**Tier:** `TIER_6_SECURITY_EVAL`  
**Slug:** `open-compass/opencompass`  
**Commit:** `e2d2b9a5236b`  
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
| Avg latency | **46.2 ms** |
| Min latency | 44.06 ms |
| Max latency | 47.52 ms |
| Samples | 5 |

### Real Tokenization Results

| Field | Value |
| ----- | ----- |
| Token count | **42** |
| Tokenization latency | 0.0 ms |
| Classification label | `LABEL_0` |
| Classification score | 0.5877 |
| Classification latency | 81.5 ms |
| Status | **PASS** |

**Input text tokenized:**
```
L_OPENCOMP (open-compass/opencompass) — 3594 files, 283247 source lines, licence Apache-2.0, primary language ['Python']
```

**First 20 tokens:**
```
['[CLS]', 'l', '_', 'open', '##com', '##p', '(', 'open', '-', 'compass', '/', 'open', '##com', '##pass', ')', '—', '35', '##9', '##4', 'files']
```

> Full MMLU/HellaSwag/TruthfulQA/ARC/Winogrande/GSM8K require dedicated GPU.
> These results are CPU inference proxy metrics using distilbert-base-uncased.

---
_Anticloud Benchmark Suite — isolation log — 2026-09-30T15:07:07.146295+00:00_