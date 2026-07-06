# `/workspace/hrtlrs` — root-level & shared resources

These sit outside the period folders and are used across projects — worth keeping/handing
over as infrastructure rather than per-project detail.

## `tools/`
A large collection of manually-installed bioinformatics software — **not** managed via
`module load` for these, so a successor needs to know it's here rather than reinstalling.
Includes (non-exhaustive): FastQC (two copies — `fastQC` and `FastQC`, check which is
actually in use), TrimGalore, eggnog-mapper 2.1.13, evigene, GFFUtils, gffread, gfftobed,
hmmer (2.3 and 3.3.2), infernal, InterProScan 5.63-95.0, KEGG tools, kraken2, Krona, Lace
(SuperTranscripts), merqury, meryl, mirdeep2, OrthoFinder, PDF-API2, randfold, RNAmmer,
RNAscan, roast, signalp (4.1 and 5.0b), tmhmm, TransDecoder, TrimGalore, Trinity
(trinityrnaseq-v2.14.0), Trinotate (two versions — `Trinotate` and
`Trinotate-Trinotate-v3.2.2`), and a Python `venv`.
- **Notes:** `bkp/` and a stray `__MACOSX/` folder (appears twice — once at `tools/` level,
  once inside `tools/bkp/`) look like leftover zip-extraction artifacts — safe to clean up.
  Worth double-checking version numbers here against whatever module system PFR uses
  before a successor assumes these are current.

## `R/x86_64-pc-linux-gnu-library/4.3`
Personal R library for R 4.3 — packages installed here won't be available if a successor
uses a different R module version. Worth listing installed packages
(`installed.packages()`) if any are non-standard/hard to reinstall (e.g. `coseq`, `fishpond`/
`swish`, `tximport` — used in the DEG/DTU scripts above).

## `slurm/checkpoint`
SLURM job checkpoint directory — likely safe to clear once no jobs are pending, but confirm
nothing is mid-run before deleting.

## `tmp_kegg_cache`
Cache directory, presumably for KEGG API lookups (e.g. via `clusterProfiler` or similar) —
safe to delete and let it rebuild.

## `workbench-k8s`
⚠️ NEEDS CONFIRMATION — Kubernetes-related, unclear purpose/whether still in use.

## `Wtmp`
⚠️ NEEDS CONFIRMATION — likely scratch/temp space; confirm nothing important lives here
before it's reclaimed.
