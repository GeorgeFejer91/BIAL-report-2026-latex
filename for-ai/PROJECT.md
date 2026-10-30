# Project contract and active handoff

## Goal and ownership

Maintain the public scientific report for BIAL grant 308/22 entirely in LaTeX. The repository is self-contained for Overleaf, with `report.tex` at its root and pdfLaTeX as its compiler. `latex/preamble.tex` owns formatting; `sections/` owns report prose, tables, numbered sources, and the separate public-summary fragment. Never regenerate these files from Word.

The user authorized a separate public report repository on 30 October 2026, with independent Git history. A private evidence archive references it as a submodule. The public project must compile without that archive, submodules, LFS, local fonts, or generated inputs.

## Active checklist

- [x] Transfer the scientific draft and public-summary fragment to editable LaTeX.
- [x] Exclude private correspondence, attachments, financial documents, and archive history.
- [x] Verify clean compilation, page limit, and rendered layout: MiKTeX pdfLaTeX, six A4 pages, no overfull boxes; every page inspected.
- [ ] Publish public main and verify Linux CI and Overleaf import behavior.

## Evidence boundaries

Preserve visible author actions and draft status. The 39-person subjective-study sample is not the PPS sample. Do not invent final PPS outcomes, ethics coverage, journal acceptance, institutional certification, or actual submission. The Research Square DOI identifies a public preprint; statistics are transcribed from the later 22 October manuscript revision recorded in the references.

The coordinated 30 October update is included across all sections and the public summary: Study 5 boundary inference is unresolved; Study 6 collection is investigator-reported as 8/24; PPS Kit is an additional methodological output. Next action: publish this verified revision and check its Linux CI. The Overleaf import link reaches login; a hosted compiler run has not been observed. Scientific completion remains dependent on author confirmations even after the formatting migration is complete.
