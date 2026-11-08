# Developer Cookbook — K_HEXSTRIKE
**Stack:** Python 3.11, scapy, PAX 27B (attack planner), AIOSS_FORMAT
**Domain:** HexStrike: authorized penetration testing framework for Anticloud infrastructure

## Authorized pentest
```python
from k_hexstrike import HexStrikeAssessor

# Authorization must be in AIOSS chain before proceeding
assessor = HexStrikeAssessor(
    target_config="./anticloud_deployment.yaml",
    pax_model="./pax-27b-q4.gguf",
    authorization_chain="./auth.aioss",
    aioss_chain="./hexstrike.aioss"
)

# Verify authorization
assessor.verify_authorization()  # raises if no valid auth entry in chain

# Generate attack plan
plan = assessor.generate_attack_plan()
print(f"Attack vectors identified: {len(plan.vectors)}")

# Execute test
results = assessor.execute_test(plan, dry_run=False)
for finding in results.findings:
    print(f"[{finding.severity}] {finding.vector}: {finding.description}")
```

## AIOSS Chain Append
```python
import hashlib, time

def aioss_append(chain_path, payload: bytes, module_id: str):
    entry_hash = hashlib.sha3_256(payload).digest()
    ts = int(time.time_ns()).to_bytes(8, 'big')
    with open(chain_path, 'rb') as f:
        f.seek(-32, 2); prev_hash = f.read(32)
    new_hash = hashlib.sha3_256(prev_hash + entry_hash + ts).digest()
    with open(chain_path, 'ab') as f:
        f.write(ts + entry_hash + new_hash)
    return new_hash.hex()
```
