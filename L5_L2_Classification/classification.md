# L5 Narrow / L2 General Classification — L_OPENCOMP
**Platform:** Anticloud | **Tier:** TIER_6_SECURITY_EVAL | **PAX:** 27B
**IP:** USPTO pending 2026, Anticloud FZ LLE, 0-1.gg | **License:** Apache-2.0

## L5 Narrow
L_OPENCOMP automates compliance evidence generation from AIOSS chains: reading chain entries, mapping them to regulatory controls, generating evidence packages, and producing compliance reports. Narrow scope: Anticloud compliance automation.

## L2 General
L2 General: L_OPENCOMP serves all regulatory frameworks across all Anticloud tiers. HIPAA for TIER_7 and NIST 800-53 for defense both use the same evidence generation engine.

## PAX 27B Integration
PAX 27B maps AIOSS chain entries to regulatory controls: 'This AIOSS entry shows PAX_INFERENCE_CORE accessed patient data — maps to HIPAA 164.312(a)(2)(i) audit log requirement.'

## AIOSS Audit Chain
Every compliance report (regulatory framework + evidence entries count + controls coverage hash + report hash) is chained: H_n = SHA3-256(H_{n-1} || entry_hash_n || timestamp_n).
Offline-verifiable, tamper-evident, zero cloud dependency.

## Regulatory / Compliance
GDPR, HIPAA, NIST 800-53, ISO 27001, FedRAMP. Automated evidence generation.
