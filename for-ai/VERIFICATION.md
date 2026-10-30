# Verification gates

Evidence must match the claim. Report missing surfaces as BLOCKED or NOT RUN.

## Local build and layout

```sh
latexmk -pdf -interaction=nonstopmode -halt-on-error -file-line-error -outdir=build report.tex
pdfinfo build/report.pdf
pdftoppm -png build/report.pdf build/page
```

Require 1–10 A4 pages, no compilation errors, overfull boxes, missing glyphs, or unresolved references. Inspect every rendered page for readable tables, clipping, and page breaks. Compilation does not validate scientific claims or imply submission.

On Windows, latexmk needs Perl. The installed Git for Windows Perl can be placed on the current process PATH. The alternative is two pdfLaTeX passes; no Perl is required for that route.

## Standalone and publication gates

For the 30 October completion task, the user authorizes local preparation and reviewable commits only. New push, Linux CI and hosted Overleaf verification are deferred, not blockers to local document preparation. The original journal portal screenshot is explicitly authorized in assets/ and the report appendix. Recheck all ten rendered scientific pages, archive hash equality and the independent source ZIP build.

- Run `powershell -NoProfile -ExecutionPolicy Bypass -File for-ai/scripts/check-context.ps1 -ProjectRoot . -RequireRemote`.
- Review explicit staged paths and all new history: no EML, attachments, finance records, account links, participant data, private local paths, or private archive objects.
- Keep report.tex and latexmkrc at the root. Only standard TeX packages and relative input paths are allowed.
- Push checked source to public main; compare local HEAD and the remote SHA.
- Verify the Linux GitHub Actions compile for that SHA and its PDF artifact.
- Inspect the public source ZIP independently of the private archive.
- Test the Open in Overleaf link. Distinguish the import/login surface from an observed Overleaf compiler run. Never claim a hosted compile based only on local or CI compilation.
