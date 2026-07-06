# hrtlrs — powerplant  handover

This repo describes the contents of my personal working directory on the `powerplant` HPC
cluster (`/output/hrtlrs`), for reference by PFR colleagues after my departure.

It does **not** contain any data or code itself — it's documentation only, describing what
lives where, why, and who else was involved, so someone can find their way around without
having to guess from folder names.

## How this is organised

There are two separate locations on `powerplant` covered here:

- **`/output/hrtlrs`** — mostly completed/archived project results, bucketed by ~1-year periods.
- **`/workspace/hrtlrs`** — active pipelines, scripts, and shared tool installs. The current
  period folder here holds work that was still **in progress** at time of departure.

| Location / Period | Doc |
|---|---|
| `/output` — 2021–2022 | [docs/2021_22.md](docs/2021_22.md) |
| `/output` — Apr 2023 – Apr 2024 | [docs/04-2023_04-2024.md](docs/04-2023_04-2024.md) |
| `/output` — Apr 2024 – Apr 2025 | [docs/04-2024_04-2025.md](docs/04-2024_04-2025.md) |
| `/output` — Apr 2025 – Apr 2026 | [docs/04-2025_04-2026.md](docs/04-2025_04-2026.md) |
| `/output` — shared/reference resources | [docs/shared-resources.md](docs/shared-resources.md) |
| `/workspace` — Apr 2025 – Apr 2026 (**active, needs a successor**) | [docs/workspace-04_2025_04_2026.md](docs/workspace-04_2025_04_2026.md) |


## Reading a project entry

Each project is listed with:
- **Collaborator(s)** — who else worked on / requested this
- **System** — species or subject
- **What it is** — one or two lines on the analysis
- **Status** — active, completed, archived, superseded
- **Notes** — anything a successor should know (gotchas, where the "real" outputs are vs. test runs, etc.)

Standard pipeline scaffolding (STAR genome indices, per-sample `fastp`/QC subfolders, `*_STARtmp`,
etc.) isn't individually documented — it's implied by the pipeline described for each project.
