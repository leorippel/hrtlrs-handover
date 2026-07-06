# hrtlrs — powerplant `/output` workspace handover

This repo describes the contents of my personal working directory on the `powerplant` HPC
cluster (`/output/hrtlrs`), for reference by PFR colleagues after my departure.

It does **not** contain any data or code itself — it's documentation only, describing what
lives where, why, and who else was involved, so someone can find their way around without
having to guess from folder names.

## How this is organised

The workspace is bucketed by ~1-year periods (roughly matching when I actively worked in
each folder), plus a handful of shared/reference resources used across projects.

| Period | Doc |
|---|---|
| 2021–2022 | [docs/2021_22.md](docs/2021_22.md) |
| Apr 2023 – Apr 2024 | [docs/04-2023_04-2024.md](docs/04-2023_04-2024.md) |
| Apr 2024 – Apr 2025 | [docs/04-2024_04-2025.md](docs/04-2024_04-2025.md) |
| Apr 2025 – Apr 2026 | [docs/04-2025_04-2026.md](docs/04-2025_04-2026.md) |
| Shared / reference resources | [docs/shared-resources.md](docs/shared-resources.md) |

## Reading a project entry

Each project is listed with:
- **Collaborator(s)** — who else worked on / requested this
- **System** — species or subject
- **What it is** — one or two lines on the analysis
- **Status** — active, completed, archived, superseded
- **Notes** — anything a successor should know (gotchas, where the "real" outputs are vs. test runs, etc.)

Entries marked **`⚠️ NEEDS CONFIRMATION`** are my best guess from folder naming and context —
please correct these before considering the doc final.

## Not covered here

Standard pipeline scaffolding (STAR genome indices, per-sample `fastp`/QC subfolders, `*_STARtmp`,
etc.) isn't individually documented — it's implied by the pipeline described for each project.
