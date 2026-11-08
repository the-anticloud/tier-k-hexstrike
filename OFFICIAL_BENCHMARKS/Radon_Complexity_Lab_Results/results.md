# Radon_Complexity_Lab_Results
**Project:** `K_HEXSTRIKE` | **Status:** `PASS` | **Run:** `2026-09-30T17:14:20.030944+00:00`

**Framework:** [Radon — Cyclomatic Complexity & Maintainability Index](https://radon.readthedocs.io/)

## Key Metrics

- **files_analyzed:** `3`
- **average_complexity:** `{'grade': 'B', 'score': 5.438976377952756}`
- **complexity_grade:** `B`
- **complexity_score:** `5.438976377952756`
- **mi_output:** `E:\fenta\Downloads\The Anticloud\TIER_6_SECURITY_EVAL\K_HEXSTRIKE\UPSTREAM\hexstrike_mcp.py - A (30.30)
E:\fenta\Downloa`

## Raw Output (first 50 lines)
```
E:\fenta\Downloads\The Anticloud\TIER_6_SECURITY_EVAL\K_HEXSTRIKE\UPSTREAM\hexstrike_mcp.py
    F 5426:0 main - B (9)
    M 150:4 HexStrikeClient.__init__ - B (6)
    C 147:0 HexStrikeClient - A (4)
    M 192:4 HexStrikeClient.safe_get - A (4)
    M 220:4 HexStrikeClient.safe_post - A (3)
    C 97:0 ColoredFormatter - A (2)
    F 267:0 setup_mcp_server - A (1)
    F 5416:0 parse_args - A (1)
    C 31:0 HexStrikeColors - A (1)
    M 116:4 ColoredFormatter.format - A (1)
    M 245:4 HexStrikeClient.execute_command - A (1)
    M 258:4 HexStrikeClient.check_health - A (1)
E:\fenta\Downloads\The Anticloud\TIER_6_SECURITY_EVAL\K_HEXSTRIKE\UPSTREAM\hexstrike_server.py
    M 3738:4 CTFToolManager.suggest_tools_for_challenge - F (92)
    F 16515:0 ctf_binary_analyzer - F (55)
    M 6159:4 CVEIntelligenceManager.analyze_cve_exploitability - F (49)
    M 6397:4 CVEIntelligenceManager.search_existing_exploits - E (39)
    M 5955:4 CVEIntelligenceManager.fetch_latest_cves - E (34)
    M 2976:4 CTFWorkflowManager._select_tools_for_challenge - E (33)
    F 9024:0 health_check - E (32)
    F 16372:0 ctf_forensics_analyzer - D (29)
    C 3492:0 CTFToolManager - D (28)
    M 7293:4 AIExploitGenerator._analyze_vulnerability_details - D (27)
    M 1003:4 IntelligentDecisionEngine.optimize_parameters - D (24)
    F 15701:0 threat_intelligence_feeds - D (23)
    M 4771:4 ParameterOptimizer._apply_technology_optimizations - D (22)
    M 6868:4 EnhancedCommandExecutor.execute - D (21)
    F 16274:0 
```

---
_Anticloud Independent Benchmark — 2026-09-30T17:14:20.030944+00:00_