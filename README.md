# 📘 DP-700 Study Notes v2 — Fabric Data Engineer Associate

Exam-focused study notes for **Microsoft DP-700: Implementing Data Engineering Solutions Using Microsoft Fabric**, rebuilt as a static HTML / CSS / JavaScript site.

[![Deploy to GitHub Pages](https://github.com/marcogrimaldi29/dp-700-study-notes-v2/actions/workflows/deploy-pages.yml/badge.svg)](https://github.com/marcogrimaldi29/dp-700-study-notes-v2/actions/workflows/deploy-pages.yml)
[![marcogrimaldi29.com](https://img.shields.io/badge/Blog-marcogrimaldi29.com-blue?logo=rss)](https://marcogrimaldi29.com)

> - 🎯 **Goal:** Earn the Microsoft Certified: Fabric Data Engineer Associate badge
> - 📅 **Aligned to:** Skills Measured effective **July 21, 2026**
> - 🌐 **Published site:** [DP-700 Study Notes v2](https://marcogrimaldi29.com/dp-700-study-notes-v2/)
> - ✍️ **Author:** [Marco Grimaldi](https://www.linkedin.com/in/marco-grimaldi29/)

---

## What's new in v2

This is a ground-up rebuild of the original [DP-700 Study Notes](https://marcogrimaldi29.com/dp-700-study-notes/):

| Change | Detail |
|--------|--------|
| **Jekyll removed** | Plain HTML + CSS + vanilla JS. No Ruby, no Gemfile, no build step — GitHub Pages serves the files directly (`.nojekyll`). |
| **Shared design system** | Same structure and component library as the [MS-102 study notes](https://marcogrimaldi29.com/ms-102-study-notes/): sticky nav, sidebar TOC with scrollspy, light/dark theme, Mermaid diagrams, callouts, decision tables. |
| **Refreshed to July 21, 2026** | Rewritten against the current official skills measured, including **Apache Airflow workspace settings**, newly listed under *Configure Microsoft Fabric workspace settings*. |
| **Corrections** | Notably the Spark vCore table — **1 CU = 2 Spark vCores** with a **3× burst factor** (F64 = 128 base / 384 burst). The v1 notes had this wrong. |
| **New depth** | Capacity smoothing and the throttling ladder, `ReadAll` vs SQL-layer security, OneLake security, query folding, SCD Type 2 two-pass MERGE, Direct Lake fallback, consumer groups, deletion vectors, `queryinsights` views, Activator and workspace monitoring. |

---

## Structure

```
dp-700-study-notes-v2/
├── index.html                        ← Home: weights, domain cards, exam overview
├── fabric-foundations/               ← Prerequisite: OneLake, capacity, engines, Delta
├── domain-1-implement-manage/        ← Domain 1 (30–35%)
├── domain-2-ingest-transform/        ← Domain 2 (30–35%)
├── domain-3-monitor-optimize/        ← Domain 3 (30–35%)
├── exam-tips/                        ← Final review: numbers, traps, checklist
├── assets/
│   ├── css/style.css                 ← Design system (Fabric palette, light/dark)
│   ├── js/main.js                    ← Header/footer injection, TOC, theme, Mermaid
│   └── images/
├── .github/workflows/deploy-pages.yml
├── .nojekyll
└── sitemap.xml
```

Each page is standalone HTML. The shared header, footer, sidebar TOC and floating buttons are injected at runtime by `assets/js/main.js`, so adding a page means writing the content and adding one entry to the `PAGES` array.

---

## Exam at a glance

| Detail | Info |
|--------|------|
| 🏅 Certification | Microsoft Certified: Fabric Data Engineer Associate |
| 📝 Passing score | **700 / 1000** (scaled) |
| ⏱️ Duration | **100 minutes** |
| ❓ Question types | MCQ, multi-select, drag-and-drop, build list, hotspot, case studies |
| 🔁 Renewal | Annual, via free online assessment on Microsoft Learn |
| 🛡️ Prerequisite | None (hands-on Fabric experience strongly recommended) |

### Domain weights

| # | Domain | Weight |
|---|--------|--------|
| 1 | Implement and manage an analytics solution | **30–35%** |
| 2 | Ingest and transform data | **30–35%** |
| 3 | Monitor and optimize an analytics solution | **30–35%** |

All three are equally weighted — balanced study across all areas is essential.

---

## Local development

No build step. Serve the folder with any static server:

```bash
npx -y serve -l 4318 .
```

Then open <http://localhost:4318>. A `.claude/launch.json` config is included for the same command.

---

## Deployment

`.github/workflows/deploy-pages.yml` publishes to GitHub Pages on push to `main` and injects the Umami analytics website ID from the `UMAMI_WEBSITE_ID` repository secret at build time, so the ID is never committed.

---

## Official resources

| Resource | Link |
|----------|------|
| 📋 Skills measured / study guide | [Official DP-700 study guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/dp-700) |
| 📄 Exam page | [DP-700](https://learn.microsoft.com/en-us/credentials/certifications/exams/dp-700/) |
| 📚 Fabric documentation | [Microsoft Fabric](https://learn.microsoft.com/en-us/fabric/) |
| 🔧 Data engineering in Fabric | [Overview](https://learn.microsoft.com/en-us/fabric/data-engineering/data-engineering-overview) |
| 🎓 Instructor-led course | [DP-700T00-A](https://learn.microsoft.com/en-us/training/courses/dp-700t00) |
| 🎬 Exam readiness | [Exam Readiness Zone](https://learn.microsoft.com/en-us/shows/exam-readiness-zone/) |

---

## Contributing

Corrections and pull requests are welcome — Fabric moves fast and some details will age. If you spot something out of date, please open an issue or PR.

⭐ If these notes helped you, consider starring the repo.

---

## Credits

Maintained by **[Marco Grimaldi](https://www.linkedin.com/in/marco-grimaldi29/)** — Cloud Solution Architect.

Created with AI assistance and reviewed by the author for accuracy and clarity. May still contain errors — always verify against the latest [Microsoft documentation](https://learn.microsoft.com/en-us/fabric/).

> *Not affiliated with or endorsed by Microsoft. For study and learning purposes only.*
