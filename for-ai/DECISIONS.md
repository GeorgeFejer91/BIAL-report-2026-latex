# Durable decisions

## D-0001 — Independent public LaTeX report

Accepted 30 October 2026. LaTeX is the sole maintained report source. The root-level report.tex uses pdfLaTeX and standard packages, with prose split into sections and shared formatting in latex/preamble.tex.

The report has independent Git history. Its private evidence archive may embed this repository as a submodule, but the public report contains no submodules and has no dependency on that archive. Private correspondence, source attachments, participant records, and financial working papers remain outside this public repository.

Overleaf ZIP import creates a copy; GitHub synchronization is an optional premium/institutional feature with manual push/pull. Both routes target this public report repository, never the private archive.
