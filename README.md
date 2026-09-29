# 📘 DP-700 Study Notes v2 — Fabric Data Engineer Associate

Free, exam-focused study notes for **Microsoft DP-700: Implementing Data Engineering Solutions Using Microsoft Fabric**.

[![marcogrimaldi29.com](https://img.shields.io/badge/Blog-marcogrimaldi29.com-blue?logo=rss)](https://marcogrimaldi29.com)

> - 🌐 **Read the notes:** **[marcogrimaldi29.com/dp-700-study-notes-v2](https://marcogrimaldi29.com/dp-700-study-notes-v2/)**
> - 📅 **Aligned to:** Skills Measured effective **21 July 2026**
> - 🎯 **Goal:** Earn the Microsoft Certified: Fabric Data Engineer Associate badge
> - ✍️ **Author:** [Marco Grimaldi](https://www.linkedin.com/in/marco-grimaldi29/)

These notes are a **companion to the official documentation**, not a replacement for it. They are written to be read in order, and they assume you will pair each section with hands-on practice in a Microsoft Fabric trial capacity.

---

## What's inside

| Section | Covers |
|---------|--------|
| [Fabric foundations](https://marcogrimaldi29.com/dp-700-study-notes-v2/fabric-foundations/) | OneLake, workspaces and domains, capacities and CUs, Lakehouse vs Warehouse vs Eventhouse, Delta Lake internals, shortcuts |
| [Domain 1 · Implement &amp; manage](https://marcogrimaldi29.com/dp-700-study-notes-v2/domain-1-implement-manage/) | Spark, domain, OneLake and Apache Airflow workspace settings; Git, database projects, deployment pipelines; the full security stack; orchestration |
| [Domain 2 · Ingest &amp; transform](https://marcogrimaldi29.com/dp-700-study-notes-v2/domain-2-ingest-transform/) | Full and incremental loads, dimensional modelling and SCDs, shortcuts and mirroring, pipelines, PySpark/T-SQL/KQL, Eventstreams, windowing |
| [Domain 3 · Monitor &amp; optimize](https://marcogrimaldi29.com/dp-700-study-notes-v2/domain-3-monitor-optimize/) | Monitoring hub and Activator alerts, error triage across seven item types, optimization for Lakehouse, pipelines, Warehouse, Eventhouse, Spark and queries |
| [Exam tips &amp; caveats](https://marcogrimaldi29.com/dp-700-study-notes-v2/exam-tips/) | Key numbers, master decision trees, the highest-yield traps, scenario→answer lookup, pre-exam checklist |

Throughout, 🎯 **caveat** callouts flag the details that most often decide a question, and every section ends with a scenario→answer table for rapid review.

---

## v1 and v2

The original [DP-700 Study Notes](https://marcogrimaldi29.com/dp-700-study-notes/) remain online. **v2 is the version to study from** — it is a ground-up rewrite against the current exam objectives.

| | v1 | v2 |
|---|---|---|
| Aligned to | Earlier skills measured | **Skills measured effective 21 July 2026** |
| Format | Markdown site (Jekyll) | Static HTML/CSS/JS — light &amp; dark theme, sidebar navigation, rendered diagrams |
| Coverage | 3 domains + prerequisites + cheatsheet | 3 domains + foundations + expanded exam-tips review |

What changed in the content:

- **Apache Airflow workspace settings** — now an explicit objective under *Configure Microsoft Fabric workspace settings*, and covered accordingly.
- **Corrected capacity figures** — the Spark vCore mapping is **1 CU = 2 Spark vCores** with a **3× burst factor** (so F64 = 128 base, 384 burst).
- **Added depth** where the exam probes hardest — capacity smoothing and the throttling ladder, why `ReadAll` bypasses SQL-layer security, OneLake security, Dataflow Gen2 query folding, the two-pass SCD Type 2 MERGE, Direct Lake fallback, streaming consumer groups, deletion vectors, the `queryinsights` views, Activator and workspace monitoring.

---

## Exam at a glance

| Detail | Info |
|--------|------|
| 🏅 Certification | Microsoft Certified: Fabric Data Engineer Associate |
| 📝 Passing score | **700 / 1000** (scaled — not 70% of questions) |
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

All three are equally weighted — there is no domain safe to skip.

---

## Official resources

| Resource | Link |
|----------|------|
| 📋 Skills measured / study guide | [Official DP-700 study guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/dp-700) |
| 📄 Exam page &amp; practice assessment | [DP-700](https://learn.microsoft.com/en-us/credentials/certifications/exams/dp-700/) |
| 📚 Fabric documentation | [Microsoft Fabric](https://learn.microsoft.com/en-us/fabric/) |
| 🔧 Data engineering in Fabric | [Overview](https://learn.microsoft.com/en-us/fabric/data-engineering/data-engineering-overview) |
| 🎓 Instructor-led course | [DP-700T00-A](https://learn.microsoft.com/en-us/training/courses/dp-700t00) |
| 🎬 Exam readiness | [Exam Readiness Zone](https://learn.microsoft.com/en-us/shows/exam-readiness-zone/) |

---

## Spotted a mistake?

Microsoft Fabric ships changes almost weekly, and features regularly move between preview and general availability — some details here **will** age. If you spot something out of date or wrong, please [report an issue](https://github.com/marcogrimaldi29/dp-700-study-notes-v2/issues).

---

## Support

If these notes helped you prepare for DP-700, there are a few ways to show it: ⭐ star this repo on GitHub so other candidates can find it, 🤝 connect with me on LinkedIn, or ☕ support the work behind them with a coffee.

<p>
  <a href="https://github.com/marcogrimaldi29/dp-700-study-notes-v2"><img src="https://img.shields.io/badge/Star_on_GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="Star on GitHub" /></a>
  <a href="https://www.linkedin.com/in/marco-grimaldi29/"><img src="https://img.shields.io/badge/Connect_on_LinkedIn-0A66C2?style=for-the-badge&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0id2hpdGUiIGQ9Ik0yMC40NDcgMjAuNDUyaC0zLjU1NHYtNS41NjljMC0xLjMyOC0uMDI3LTMuMDM3LTEuODUyLTMuMDM3LTEuODUzIDAtMi4xMzYgMS40NDUtMi4xMzYgMi45Mzl2NS42NjdIOS4zNTFWOWgzLjQxNHYxLjU2MWguMDQ2Yy40NzctLjkgMS42MzctMS44NSAzLjM3LTEuODUgMy42MDEgMCA0LjI2NyAyLjM3IDQuMjY3IDUuNDU1djYuMjg2ek01LjMzNyA3LjQzM2EyLjA2MiAyLjA2MiAwIDAgMS0yLjA2My0yLjA2NSAyLjA2NCAyLjA2NCAwIDEgMSAyLjA2MyAyLjA2NXptMS43ODIgMTMuMDE5SDMuNTU1VjloMy41NjR2MTEuNDUyek0yMi4yMjUgMEgxLjc3MUMuNzkyIDAgMCAuNzc0IDAgMS43Mjl2MjAuNTQyQzAgMjMuMjI3Ljc5MiAyNCAxLjc3MSAyNGgyMC40NTFDMjMuMiAyNCAyNCAyMy4yMjcgMjQgMjIuMjcxVjEuNzI5QzI0IC43NzQgMjMuMiAwIDIyLjIyNSAweiIvPjwvc3ZnPg%3D%3D" alt="Connect on LinkedIn" /></a>
  <a href="https://buymeacoffee.com/marcogrimaldi29"><img src="https://img.shields.io/badge/Support_with_a_coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black" alt="Support with a coffee" /></a>
</p>

---

## Credits &amp; disclaimer

Maintained by **[Marco Grimaldi](https://www.linkedin.com/in/marco-grimaldi29/)** — Cloud Solution Architect. More certification guides and tech writing at **[marcogrimaldi29.com](https://marcogrimaldi29.com)**.

Created with AI assistance and reviewed by the author for accuracy and clarity. These notes contain **no exam content** and are an independent study aid for learning purposes only. They may still contain errors — always verify against the latest [Microsoft documentation](https://learn.microsoft.com/en-us/fabric/) and the current [DP-700 study guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/dp-700).

> *Not affiliated with or endorsed by Microsoft.*
