# Deploy Guide — K_HEXSTRIKE
**Tier:** TIER_6_SECURITY_EVAL | **Stack:** Python 3.11, scapy, PAX 27B (attack planner), AIOSS_FORMAT
**Air-gap capable after initial setup.**

## Prerequisites
Python 3.11+, scapy 2.5+, PAX 27B. AUTHORIZED DEPLOYMENT ONLY — requires signed authorization in AIOSS chain.

## Environment
AUTHORIZED TESTING ENVIRONMENT ONLY. PAX 27B for attack planning. No GPU required for most tests.

## AIOSS Integration
```bash
aioss init --module K_HEXSTRIKE --output ./k_hexstrike.aioss
aioss append --chain ./k_hexstrike.aioss --payload ./output.bin --module K_HEXSTRIKE
aioss verify --chain ./k_hexstrike.aioss
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
    module="K_HEXSTRIKE",
    aioss_chain="./K_HEXSTRIKE.aioss",
    classification="L5_NARROW_L2_GENERAL"
)
result = harness.process(input_data)
```

## Verification
```bash
aioss verify --chain ./K_HEXSTRIKE.aioss --verbose
python -m K_HEXSTRIKE.tests.smoke
```
