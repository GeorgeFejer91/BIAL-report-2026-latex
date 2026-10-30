# BIAL 2026 scientific report

LaTeX author-review draft for **grant 308/22 â€” Altered States of Viscereality**.

**[Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https%3A%2F%2Fgithub.com%2FGeorgeFejer91%2FBIAL-report-2026-latex%2Farchive%2Frefs%2Fheads%2Fmain.zip)** Â· [Download source ZIP](https://github.com/GeorgeFejer91/BIAL-report-2026-latex/archive/refs/heads/main.zip)

The Overleaf link imports a new copy. Set **Main document: `report.tex`** and **Compiler: pdfLaTeX**, then Recompile. Alternatively upload the source ZIP using **New project â†’ Upload project**. Use the current TeX Live version offered by Overleaf. No local paths, private files, external fonts, shell escape, Python, or bibliography service are needed to compile.

For ongoing synchronization, use **New project â†’ GitHub repo** and select this repository. This requires Overleaf's GitHub synchronization feature (premium or qualifying institutional access); push/pull is manual. ZIP import does not create a synchronized project. See [Overleaf's GitHub instructions](https://docs.overleaf.com/integrations-and-add-ons/git-integration-and-github-synchronization/github-synchronization) and [main-document guidance](https://docs.overleaf.com/getting-started/recompiling-your-project/the-main-document).

## Editing and compiling

```text
report.tex                    main document, at the project root
latex/preamble.tex            shared LaTeX formatting
sections/aims.tex              aims and implementation
sections/methods.tex           study methods and author actions
sections/results-discussion.tex
sections/conclusions.tex       conclusions and output indicators
sections/references.tex        numbered sources and public DOI links
sections/public-summary.tex    separate fragment for the official template
latexmkrc                     pdfLaTeX defaults
```

Edit these `.tex` files directly. LaTeX is the sole maintained report source. The public-summary fragment is not included in the scientific report's page count.

```sh
latexmk -pdf -interaction=nonstopmode -halt-on-error -outdir=build report.tex
```

Or run `pdflatex -interaction=nonstopmode -halt-on-error report.tex` twice. The first command writes `build/report.pdf`; the fallback writes `report.pdf`. GitHub Actions also compiles on Linux and provides a downloadable PDF artifact.

## Scientific status and publication boundary

This is an **author-review draft**, not a submitted or approved final report. Final peripersonal-space results, ethics/reporting-period confirmation, journal status, and bibliographic checks remain open. The scientific report must stay within 10 pages.

The Research Square preprint is [10.21203/rs.3.rs-10842634/v1](https://doi.org/10.21203/rs.3.rs-10842634/v1). The transcribed results use a later manuscript snapshot, identified in the references; they have not been newly analyzed or revalidated against that preprint.

This repository has independent history and contains report text only. Emails, contracts, finance records, participant-level records, source attachments, and private archive history are excluded. Internal sources are described without reproducing correspondence. The public repository has no submodules and does not require access to its private parent.

Agent context: [for-ai/README.md](for-ai/README.md).
