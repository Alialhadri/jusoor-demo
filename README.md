<p align="center">
  <img src="jusoor-logo.svg" width="240" alt="Jusoor — جسور"/>
</p>

<h1 align="center">Jusoor — Diabetes Care Platform (demo)</h1>
<p align="center"><b>Team-based diabetes care across 5 primary health centers · بالعربية والإنجليزية</b><br/>
Type 1 · Type 2 · Gestational — one self-contained file, no build step.</p>

---

## What this is
A **single self-contained `index.html`** demo of the Jusoor programme, styled as a production-grade
clinical platform (MOH/Raqeem-class look & feel). Open it by double-click, or host it free on GitHub Pages.
No npm, no build, no framework.

## What's new in this version
- **Full Arabic / English UI** — one-click عربي/EN toggle, complete RTL layout, Arabic patient names,
  Arabic clinical recommendations, Hijri + Gregorian dates.
- **Role-based sign-in** — Care Coordinator / Physician / Educator / Programme Lead each land on their
  own view (demo session; production path is Nafath SSO, stated in-app).
- **Real outcomes & trends** — every patient carries a **dated HbA1c history**; the Trends page
  aggregates those measurements per quarter (mean HbA1c, % at target, % high-risk, per-center lines).
  No simulated curves.
- **Team Worklist (close the loop)** — every open care gap becomes an assignable task with an
  **assignee, due date, overdue flag and completion state**.
- **Lost-to-follow-up queue** — patients with no contact ≥ 90 days, with one-click Arabic SMS/WhatsApp
  recall and a "Contacted" action that closes the loop.
- **Methodology page** — every risk weight and recommendation mapped to its guideline basis
  (ADA Standards of Care 2026, KDIGO 2024), with stated limitations and a pilot validation plan
  (UKPDS/RECODe comparison, SFDA SaMD pathway).
- **Integration & compliance page** — NPHIES, Raqeem, Mawid, Wasfaty, Sehhaty, Nafath integration
  phases, and the PDPL / NCA ECC / SFDA posture.
- **Versioned data schema (v3)** — localStorage with schema version + migration, so saved panels
  survive app updates. Auto-imports data from the older v2 demo if present in the same browser.

## Carried over from v2
- One single registry, 5 centers with side-by-side comparison, reactive live-risk enrolment form,
  medication-aware risk engine, physician pre-visit summaries, educator tracking, morning huddle,
  JSON export/import, comorbidities per patient.

## Try it locally
Open `index.html` in any browser (double-click). Sign in with any role.

## Put it live on GitHub Pages (no build)
1. Push these files to the repo root (see `PUSH_TO_GITHUB.md`).
2. Repo → **Settings → Pages → Source: Deploy from a branch → `main` → `/ (root)` → Save**.
3. Live at `https://alialhadri.github.io/jusoor-demo/`.

## Your exact logo
The header uses **`jusoor-logo.png`** if present, falling back to `jusoor-mark.svg`. Drop your
pixel-exact `jusoor-logo.png` into this folder — no code change needed.

## Disclaimer
Decision-support demo only — **not medical advice**. 100% synthetic data, no PHI. Clinical logic
requires validation and regulatory review (SDAIA / SFDA / PDPL) before any real-world care use.

© 2026 Jusoor (جسور).
