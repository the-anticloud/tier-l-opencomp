# 3-Seed Simulation — L_OPENCOMP

**Seeds:** `53706` · `85043` · `19242`

**Seed method:** `sha256("L_OPENCOMP")[:8]` as hex→int, offsets +0 / +31337 / +65536

> These seeds are deterministic and documented. Any researcher can reproduce this simulation exactly by running `write_three_seed_simulation.py` with project name `L_OPENCOMP`.

## Confidence Intervals (mean ± σ across 3 seeds)

| Metric | Mean | σ | 95% CI |
|--------|------|---|--------|
| trl_score | 6.846 | 0.1103 | ±0.2162 |
| throughput_tokens_per_sec | 4788.5333 | 33.3619 | ±65.3893 |
| p50_latency_ms | 45.5933 | 4.454 | ±8.7298 |
| p99_latency_ms | 113.0033 | 6.4043 | ±12.5524 |
| ttft_ms | 28.4067 | 1.2422 | ±2.4347 |
| mmlu_proxy | 0.7161 | 0.0304 | ±0.0596 |
| hellaswag_proxy | 0.7956 | 0.0264 | ±0.0517 |
| truthfulqa_proxy | 0.5415 | 0.0204 | ±0.04 |
| arc_proxy | 0.6795 | 0.0467 | ±0.0915 |
| complexity_cyclomatic | 4.0867 | 0.2894 | ±0.5672 |
| maintainability_index | 66.2633 | 4.1201 | ±8.0754 |
| security_issues_high | 0.3333 | 0.4714 | ±0.9239 |
| dependency_freshness_pct | 74.6333 | 2.2647 | ±4.4388 |
| test_coverage_pct | 66.6667 | 3.7748 | ±7.3986 |
| doc_coverage_pct | 61.5 | 6.4689 | ±12.679 |
| memory_mb | 102.5333 | 7.6111 | ±14.9178 |
| gpu_util_pct | 71.3 | 5.0259 | ±9.8508 |
| openssf_score | 6.1233 | 0.531 | ±1.0408 |
| eu_ai_act_compliance_pct | 79.7667 | 6.3908 | ±12.526 |
| slsa_level | 1.6667 | 0.4714 | ±0.9239 |

## Per-Seed Raw Results

| Metric | Seed 53706 | Seed 85043 | Seed 19242 |
|--------|------------|------------|------------|
| trl_score | 6.753 | 6.784 | 7.001 |
| throughput_tokens_per_sec | 4741.7 | 4807.0 | 4816.9 |
| p50_latency_ms | 51.88 | 42.11 | 42.79 |
| p99_latency_ms | 106.97 | 110.17 | 121.87 |
| ttft_ms | 27.03 | 30.04 | 28.15 |
| mmlu_proxy | 0.7376 | 0.7375 | 0.6731 |
| hellaswag_proxy | 0.7655 | 0.8297 | 0.7916 |
| truthfulqa_proxy | 0.5683 | 0.5375 | 0.5188 |
| arc_proxy | 0.6649 | 0.6311 | 0.7426 |
| complexity_cyclomatic | 4.33 | 4.25 | 3.68 |
| maintainability_index | 63.32 | 72.09 | 63.38 |
| security_issues_high | 0 | 0 | 1 |
| dependency_freshness_pct | 72.3 | 77.7 | 73.9 |
| test_coverage_pct | 64.2 | 63.8 | 72.0 |
| doc_coverage_pct | 54.7 | 59.6 | 70.2 |
| memory_mb | 93.6 | 112.2 | 101.8 |
| gpu_util_pct | 77.3 | 71.6 | 65.0 |
| openssf_score | 5.55 | 6.83 | 5.99 |
| eu_ai_act_compliance_pct | 88.8 | 75.0 | 75.5 |
| slsa_level | 2 | 2 | 1 |

---
_Anticloud 3-Seed Simulation — 2026-09-30T16:01:40.704491+00:00_
_Citation: Lois-Kleinner. (2026). The Anticloud. DOI: pending._