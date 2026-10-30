# BIAL 308/22 scientific final report

LaTeX source for the scientific report at the **30 October 2026 cutoff**. It documents completed outputs and unfinished work. It does not claim journal acceptance, Foundation approval or submission.

The report is self-contained and limited to ten pages, including references and the investigator-authorized original journal-status screenshot. Private contracts, correspondence, finance records and participant-level data are excluded.

## Build

Run pdfLaTeX twice from this directory:

```sh
pdflatex -no-shell-escape -interaction=nonstopmode -halt-on-error report.tex
pdflatex -no-shell-escape -interaction=nonstopmode -halt-on-error report.tex
```

Alternatively use `latexmk -pdf -outdir=build report.tex`. Standard TeX Live or MiKTeX packages suffice. No private parent, submodule, local font, external service or bibliography processor is needed.

For Overleaf, upload the source ZIP and choose **report.tex / pdfLaTeX**. [Import published main](https://www.overleaf.com/docs?snip_uri=https%3A%2F%2Fgithub.com%2FGeorgeFejer91%2FBIAL-report-2026-latex%2Farchive%2Frefs%2Fheads%2Fmain.zip) imports the published branch, which may precede a locally prepared revision. GitHub synchronization requires the corresponding Overleaf account feature and manual synchronization. A local compile is not an observed hosted compile.

## Source ownership

- `report.tex`: scientific report entry point.
- `sections/`: narrative, comparison/results tables, references and screenshot appendix.
- `sections/public-summary.tex`: separate public-results text, outside scientific page count.
- `latex/preamble.tex`: shared typography.
- `assets/journal-status-original.png`: unaltered user-supplied screenshot, explicitly approved for inclusion.

Results use the public [Research Square v1 preprint](https://doi.org/10.21203/rs.3.rs-10842634/v1) and supplement, with later withdrawn endpoints excluded. Study 5 uses the documented current analysis amendments; Study 6 distinguishes eight participants with both mappings from three partial questionnaire records and target 24. Official forms, finance certification and portal submission belong to the private preparation package.

Current work is prepared on a local review branch. No new push or CI/Overleaf-hosted build is claimed. Agent context starts at [for-ai/README.md](for-ai/README.md).
