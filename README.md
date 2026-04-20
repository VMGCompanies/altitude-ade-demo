# Altitude Home Loans — Autonomous Digital Employee Platform

A Fortune 500-grade enterprise platform prototype housing the **Dynamic Loan Processor ADE** that executes Altitude's actual operational playbooks — the **JP File Set-Up Checklist** and the **Processor Closing Checklist** — autonomously, end-to-end, anchored to LQB.

**Live demo:** https://vmgcompanies.github.io/altitude-ade-demo/

---

## What the demo shows

- **Command Center** with live-streaming ADE activity across 44 loans (Arizona-weighted, product-diverse)
- **Dynamic Loan Processor ADE** with 36 Altitude-specific capabilities across 7 domains, 14 integration connections, 11 guardrails, 24/7 schedule, live decision log
- **Loan Pipeline** grid → **Loan Detail** drill-down with both full checklists rendered item-by-item, per-item ADE work product (document, rule, extracted fields, LQB reference), re-run / override controls
- **Workflows** DAG across three phases (File Set-Up → Processing → Pre-Close, 33 nodes) with node-level success rates, policies, recent runs
- **Playbooks** reference — both checklists verbatim + 6 loan-product variants (VA+PUD, Manufactured, FHA, Refi Rate/Term, Cash-Out, Purchase Conv)
- **Documents & Data** inbox with full extraction viewer (bounding boxes on document preview, editable key/value pairs with per-field confidence)
- **Communications** — unified inbox (~220 threads), Master List submissions with correct Altitude subject-line convention, templates library with live variable preview
- **Analytics** — cycle time / cost per loan / automation rate / throughput / accuracy / utilization, plus an editable ROI calculator
- **Audit & Governance** — hash-chained immutable log, 14 policies, 7-regulation compliance matrix (RESPA / TRID / ECOA / FCRA / SAFE / HMDA / HOEPA)
- **Settings** — integrations, 5-role access control with users, notification rules, billing & usage

The Altitude mortgagee clause — **Altitude Financial Corporation, ISAOA/ATIMA, 1885 N Kolb Rd, Tucson AZ 85715** — is referenced verbatim throughout the platform on CPL / Prelim / Hazard / Flood / HO6 / Master Policy verifications.

---

## Phase-by-phase versions

Each phase is a standalone, runnable HTML file:

| Phase | File | Scope |
|-------|------|-------|
| 1 | [phase1.html](phase1.html) | Foundation, shell, brand system, 44-loan data model, simulation engine, Command Center |
| 2 | [phase2.html](phase2.html) | Pipeline Heatmap, Today's Exceptions, Digital Employees roster + Loan Processor profile |
| 3 | [phase3.html](phase3.html) | Loan Pipeline grid + Loan Detail drill-down (checklists, 1003, docs, timeline, conditions, comms, decisions) |
| 4 | [phase4.html](phase4.html) | Workflows DAG + Playbooks reference, Documents extraction viewer, Communications inbox + Templates |
| 5 | [phase5.html](phase5.html) / [index.html](index.html) | Analytics + ROI calculator, Audit & Governance, Settings (integrations, access, notifications, billing) |

---

## Technical notes

- Single-file HTML per phase · React 18 + Babel + Tailwind + Recharts + lucide via CDN
- No backend, no build step — open in any modern browser
- All state is in-memory React; simulation runs via `setInterval`
- Altitude Home Loans logo fetched from their site with a clean mountain-mark SVG fallback

Built for Neuralogic as a rapid prototype for a live sales demo.
