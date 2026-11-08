# L5 Narrow / L2 General Classification — K_HEXSTRIKE
**Platform:** Anticloud | **Tier:** TIER_6_SECURITY_EVAL | **PAX:** 27B
**IP:** USPTO pending 2026, Anticloud FZ LLE, 0-1.gg | **License:** Apache-2.0

## L5 Narrow
K_HEXSTRIKE provides authorized penetration testing capabilities for Anticloud deployments. Narrow scope: Anticloud infrastructure pentesting only — API endpoints, AIOSS chain integrity, PAX harness security, container security. Not a general-purpose offensive tool.

## L2 General
L2 General: K_HEXSTRIKE tests all Anticloud tiers for vulnerabilities before production deployment. Same pentesting framework for hospital and defense deployments.

## PAX 27B Integration
PAX 27B generates attack plans: given an Anticloud deployment configuration, PAX identifies likely attack vectors and generates a structured pentesting plan. All attack activities are AIOSS-chained for authorization audit.

## AIOSS Audit Chain
Every pentest event (target hash + attack vector hash + finding hash + severity + remediation recommendation) is chained: H_n = SHA3-256(H_{n-1} || entry_hash_n || timestamp_n).
Offline-verifiable, tamper-evident, zero cloud dependency.

## Regulatory / Compliance
NIST SP 800-115 (security testing). CVE, OWASP. Authorized pentesting only.
