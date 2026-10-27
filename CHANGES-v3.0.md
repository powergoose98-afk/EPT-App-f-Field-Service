# Test Bench v3.0 — ATS-2025 alignment

## Section numbers fixed
- lvswgr, mvswgr: 7.1 → 7.1.1 · panel: 7.1 → 7.1.2
- netprot: 7.6.3 → **7.8** · mvvac: 7.6.2 → **7.6.3** (SF6 stays 7.6.4) · mvair oil: 7.6.5 → **7.6.2**
- recloser: 7.6.6 → **7.24.1 / 7.24.2**
- regulator: 7.2.3 → **7.12.1.1** (LTC 7.12.3)
- lvcable: 7.3.1 → **7.3.2** · mvcable: 7.3.2 → **7.3.3**
- outdoor bus: 7.4 → **7.21** · ups: 7.21 → **7.22.2** · dcmach: 7.15.2 → **7.15.3**
- cap/reactors: 7.20.2 → **7.20.3.x** (7.20.2 is reserved)
- firepump: no ATS section (old cite was UPS 7.22.2) → NFPA 20 / 25
- Fluid limits: Table 100.14 → **Table 100.4** (100.14 is the IR temperature-correction chart)

## Content
- Every test now has the manual's acceptance value (blue box), the clause it came from, and an "Optional" badge where ATS marks it with an asterisk.
- Tests and inspection items added, removed, or reworded to match each section (e.g., control-wiring IR, CT-circuit current injection, network-protector fuse/relay/trip-actuator checks, MV breaker vacuum-bottle and contact timing, GFP pickup/timing/55%–80% control-voltage trip).
- Tables read from page images and entered: 100.1, 100.3, 100.5, 100.6.3, 100.6.7, 100.7, 100.8, 100.9, 100.10, 100.11, 100.13, 100.18, 100.19, 100.20.

## Flagged "Check against your manual"
The ATS-2025 copy used was missing printed pp. 45–57, 59–62, 235. Affected: 7.2.1.2 (after B.3), 7.2.2, 7.3.2, 7.3.3 text, 7.4, start of 7.5.1.1, Table 100.2. Those entries carry a note in the app. Also flagged: firepump (no ATS section), sysfunc (Section 8 defers to ANSI/NETA ECS), cap (liquid-filled reactors and resistors not itemized).

## Not changed / not covered
- Maintenance (MTS) and Troubleshoot tabs: content untouched (MTS standard was not in the PDF).
- Not added: 7.7 circuit switchers, 7.25 fiber optic, 7.26 EV charging, 7.27 arc-energy reduction (only referenced under relays), 7.28 BESS, 7.29 PV, Sections 10–11.

## Packaging
- Icons moved into `icons/` (the manifest, service worker, and page already pointed there).
- Service worker caches each file separately so one missing file can't break offline install; cache bumped to `test-bench-v13-glass-ats2025`.
