# Shared / reference resources

These aren't individual projects — they're reusable reference data/tools used across
multiple projects above. Whoever inherits this workspace will likely want to keep these.

## `AnnoDB_V1`
Custom Bioconductor-style annotation packages (`org.*.eg.db`) for:
- *Actinidia chinensis* (Red5) — `org.Achinensis.eg.db`
- *Malus domestica* — `org.Mdomestica.eg.db`
- *Nicotiana benthamiana* — `org.Nbenthamiana.eg.db`
- *Solanum lycopersicum* (tomato) — `org.Slycopersicum.eg.db`
- *Solanum tuberosum* (potato) — `org.Stuberosum.eg.db`

First-generation annotation DBs — superseded by `AnnoDB_V2` for species present in both.

## `AnnoDB_V2`
Updated annotation packages, additional species/genome versions:
- *Actinidia chinensis* CK51-09 and Red5v2 assemblies
- *Malus domestica* GDDH13 1.1
- *Nicotiana tabacum* (Sierro assembly)
- *Prunus persica* v2 (peach)
- *Solanum lycopersicum* ITAG4
- *Solanum tuberosum* DM 1.3

Also includes shared `BLAST`, `Emapper` (eggNOG-mapper), and raw `Fasta_files` used to build
these DBs — useful if a successor needs to rebuild or extend one.

## `OrthoFinder`
Proteome sets (`primary_transcripts`) prepared for OrthoFinder orthology analysis — check
whether this was a one-off run or a resource meant to be reused/extended across projects.

## `Rdata`
R code for Anno repo.
