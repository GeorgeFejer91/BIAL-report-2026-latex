# Project contract and active handoff

## Goal and ownership

Maintain the public scientific report for BIAL grant 308/22 entirely in LaTeX. The repository is self-contained for Overleaf, with `report.tex` at its root and pdfLaTeX as its compiler. `latex/preamble.tex` owns formatting; `sections/` owns report prose, tables, numbered sources, and the separate public-summary fragment. Never regenerate these files from Word.

The user authorized a separate public report repository on 30 October 2026, with independent Git history. A private evidence archive references it as a submodule. The public project must compile without that archive, submodules, LFS, local fonts, or generated inputs.

## Active checklist

- [x] Transfer the scientific draft and public-summary fragment to editable LaTeX.
- [x] Exclude private correspondence, attachments, financial documents, and archive history.
- [x] Verify clean compilation, page limit, and rendered layout: MiKTeX pdfLaTeX, five A4 pages, no overfull boxes; every page inspected.
- [ ] Publish public main and verify Linux CI and Overleaf import behavior.

## Evidence boundaries

Preserve visible author actions and draft status. The 39-person subjective-study sample is not the PPS sample. Do not invent final PPS outcomes, ethics coverage, journal acceptance, institutional certification, or actual submission. The Research Square DOI identifies a public preprint; statistics are transcribed from the later 22 October manuscript revision recorded in the references.

Next action: compile and inspect the PDF, then publish the checked source. Scientific completion remains dependent on author confirmations even after the formatting migration is complete.
