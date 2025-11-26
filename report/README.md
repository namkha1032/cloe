# Report Templates for Assignment 3

This folder contains LaTeX skeletons and supporting files for writing your technical report for Assignment 3 (Deep Learning for Blood-Cell Classification).

Important notes:

- Use either the CVPR (two-column) or ICLR (one-column) LaTeX template provided here as a starting point. Do not modify default template settings (font size, margins, etc.).
- Page limit is 6 pages (excluding references). Keep the main text within this limit.
- Do not include any AI-generated substantive content; AI may be used only for proofreading and grammar checks per the assignment rules.
- Do not modify `class_map.json` or the dataset files.

Files included:

- `CVPR_report.tex` - Two-column CVPR-styled skeleton with section placeholders required by the assignment.
- `ICLR_report.tex` - One-column ICLR-styled skeleton with section placeholders.
- `references.bib` - Example BibTeX file with a few entries to get started.
- `figures/` - Folder to store images/figures used in the report.

How to compile:

- Recommended: compile with `pdflatex` and `bibtex` (or `biber` if you change bibliography backend).
- Example commands (macOS / zsh):

```bash
pdflatex CVPR_report.tex
bibtex CVPR_report
pdflatex CVPR_report.tex
pdflatex CVPR_report.tex
```

or for `ICLR_report.tex`:

```bash
pdflatex ICLR_report.tex
bibtex ICLR_report
pdflatex ICLR_report.tex
pdflatex ICLR_report.tex
```

If you prefer to use Overleaf, upload the entire `report/` folder there and compile using Overleaf's compiler.

Contact:

If you want, I can also: 
- Fill the Method section with a starter description of a CNN model implemented from scratch in PyTorch. 
- Add a small figure example and a sample results table.

Tell me which extra items you'd like.
