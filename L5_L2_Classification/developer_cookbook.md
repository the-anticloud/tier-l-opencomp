# Developer Cookbook — L_OPENCOMP
**Stack:** Python 3.11, AIOSS_FORMAT, PAX 27B, reportlab, AIOSS_FORMAT
**Domain:** OpenComp: compliance automation — auto-generate evidence from Anticloud AIOSS chains

## Auto-generate compliance evidence
```python
from l_opencomp import OpenCompGenerator

generator = OpenCompGenerator(
    pax_model="./pax-27b-q4.gguf",
    chains_dir="./aioss_chains/",
    aioss_chain="./opencomp.aioss"
)

# HIPAA evidence package
package = generator.generate(
    framework="HIPAA",
    period_start="2026-01-01",
    period_end="2026-03-31"
)
print(f"Controls covered: {package.controls_covered}/{package.controls_total}")
print(f"Evidence PDF: {package.pdf_path}")
print(f"Chain: {package.chain_hash}")
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
