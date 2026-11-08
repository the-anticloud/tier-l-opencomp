# Deploy Guide — L_OPENCOMP
**Tier:** TIER_6_SECURITY_EVAL | **Stack:** Python 3.11, AIOSS_FORMAT, PAX 27B, reportlab, AIOSS_FORMAT
**Air-gap capable after initial setup.**

## Prerequisites
Python 3.11+, PAX 27B, reportlab 4.1+, all AIOSS chains (read access).

## Environment
4GB RAM. CPU for evidence mapping. GPU for PAX regulatory analysis.

## AIOSS Integration
```bash
aioss init --module L_OPENCOMP --output ./l_opencomp.aioss
aioss append --chain ./l_opencomp.aioss --payload ./output.bin --module L_OPENCOMP
aioss verify --chain ./l_opencomp.aioss
```

## Air-Gap Setup
```bash
pip download -r requirements.txt -d ./wheels/
pip install --no-index --find-links ./wheels/ -r requirements.txt
```

## PAX 27B Harness Wiring
```python
from anticloud_pax import PAXHarness
harness = PAXHarness(
    model_path="./pax-27b-q4.gguf",
    module="L_OPENCOMP",
    aioss_chain="./L_OPENCOMP.aioss",
    classification="L5_NARROW_L2_GENERAL"
)
result = harness.process(input_data)
```

## Verification
```bash
aioss verify --chain ./L_OPENCOMP.aioss --verbose
python -m L_OPENCOMP.tests.smoke
```
