# STEP 01 REPORT: OSINT Deployment - VPN Corporate Ownership Investigation

**Task ID:** PANOPTICON-VPN-001
**Step:** 01 of 12
**Status:** ✅ COMPLETE
**Timestamp:** 2026-03-17 02:09:56 UTC
**Agent:** osint_specialist

---

## WHAT WAS DONE

Deployed `osint_specialist` agent to execute Phase 1 data acquisition for Vector Alpha (Corporate Unmasking & UBOs). The agent was tasked with tracing corporate ownership chains for major VPN holding companies and identifying Ultimate Beneficial Owners (UBOs).

### Investigation Targets
1. **Kape Technologies** - ExpressVPN, CyberGhost, PIA, ZenMate
2. **NordSec / Tesonet** - NordVPN, Surfshark
3. **Ziff Davis (J2 Global)** - IPVanish, StrongVPN, SaferVPN
4. **Pango / AnchorFree** - Hotspot Shield, Betternet, Super VPN
5. **Novator Partners** - Nord Security investor

---

## PHYSICAL PROOF

### File Created:
```
/a0/usr/workdir/task_20260317_012233_panopticon-vpn-deanonymization/raw_data/01_osint_kape_nordsec_findings.json
```

### File Statistics:
```
-rw-r--r-- 1 root root 13402 Mar 17 02:09 01_osint_kape_nordsec_findings.json
Size: 13,402 bytes
Lines: 300
```

### Data Sources Verified:
- Wikipedia OSINT documents: 9 sources
- Corporate registry references: Multiple jurisdictions
- SEC filing references: Ziff Davis (NASDAQ: ZD)

---

## KEY FINDINGS

### 1. KAPE TECHNOLOGIES - ✅ UBO RESOLVED
| Field | Finding |
|-------|--------|
| **Ultimate Beneficial Owner** | **Teddy Sagi** (Israeli billionaire, $7.1B net worth) |
| **Ownership Chain** | Teddy Sagi → Unik Holdings → Kape Technologies |
| **VPN Subsidiaries** | ExpressVPN, CyberGhost, PIA, ZenMate, Intego, Webselenese |
| **Jurisdiction** | Israel/UK (delisted from AIM London 2021) |
| **Intelligence Risk** | ⚠️ HIGH - 1996 fraud/bribery conviction (5 months prison), Pandora Papers exposure, Cypriot golden visa |

### 2. NORDSEC / TESONET - ✅ UBO RESOLVED
| Field | Finding |
|-------|--------|
| **Ultimate Beneficial Owners** | **Tomas Okmanas** & **Eimantas Sabaliauskas** |
| **Ownership Chain** | Tesonet → Nord Security (Novator Partners $100M funding) |
| **VPN Subsidiaries** | NordVPN, Surfshark (merged 2022) |
| **Jurisdiction** | Amsterdam (parent), Panama (operations), Lithuania (Tesonet HQ) |
| **Intelligence Risk** | ⚠️ MEDIUM - Lithuanian government "National Patrons" status 2024, Panama opacity jurisdiction |

### 3. ZIFF DAVIS (J2 GLOBAL) - ⚠️ PARTIAL
| Field | Finding |
|-------|--------|
| **Ownership** | Public shareholders (NASDAQ: ZD) |
| **VPN Subsidiaries** | IPVanish, StrongVPN, SaferVPN, Encrypt.me, NetProtect, VIPRE |
| **Gap** | Requires SEC 13F filing analysis for institutional shareholders |

### 4. PANGO / ANCHORFREE - ❌ OPEN
| Field | Finding |
|-------|--------|
| **VPN Subsidiaries** | Hotspot Shield, Betternet, Super VPN |
| **Jurisdiction** | USA (Redwood City, CA) + Ukraine office |
| **Gap** | No public UBO information - requires deeper investigation |

### 5. NOVATOR PARTNERS - ❌ OPEN
| Field | Finding |
|-------|--------|
| **Role** | Led $100M funding round for Nord Security (April 2022) |
| **Known Partner** | Birgir Ragnarson |
| **Gap** | Investment firm ownership structure unknown - need LP identification |

---

## INTELLIGENCE CORRELATION ALERTS

### Pattern: Multi-Jurisdictional Opacity
- Kape: Israel → Cyprus → UK (golden visa + offshore structures)
- NordSec: Lithuania → Netherlands → Panama (tech hub + tax haven)
- Both patterns indicate deliberate jurisdictional arbitrage

### Pattern: State Recognition
- Tesonet founders awarded "National Patrons" by Lithuanian government 2024
- Suggests potential state-level cooperation or recognition

### Pattern: Infrastructure Convergence
- Tesonet controls: Oxylabs (proxy), Hostinger (hosting), NordVPN/Surfshark (VPNs)
- Comprehensive data collection capability across multiple services

### Pattern: Review Site Capture
- Kape owns Webselenese (VPN review publisher)
- Conflict of interest: VPN owner controlling "independent" reviews

---

## VERIFICATION RESULTS

### ✅ Verified Findings:
1. Teddy Sagi ownership of Kape Technologies confirmed via multiple sources
2. Tesonet founder identities confirmed with biographical details
3. NordVPN/Surfshark merger confirmed (2022)
4. Kape acquisition of ExpressVPN, CyberGhost, PIA confirmed
5. Kape delisting from AIM London (2021) confirmed

### ⚠️ Requires Further Investigation:
1. Ziff Davis institutional shareholders (SEC 13F)
2. Pango/AnchorFree UBO structure
3. Novator Partners LP identification
4. Cross-reference executives with intelligence agencies

---

## NEXT STEPS

**Step 02:** Deploy `browser_agent` for dynamic web scraping of additional VPN corporate pages
**Step 03:** Ingest all raw data into structured JSON format
**Step 04:** Process VPN ownership chains via `id_data_analyst`

---

## EVIDENCE INTEGRITY

All findings backed by verifiable sources documented in the JSON output. No simulated or fabricated data.

---

**Report Status:** COMPLETE
**Next Action:** Proceed to Step 02

---
*Report generated: 2026-03-17 02:15:00 UTC*
*Authority: AlexH | APEX PRIME DIRECTIVE*
