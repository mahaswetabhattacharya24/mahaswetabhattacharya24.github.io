# Resume Sources

Polished resume targeting AI/ML Research Scientist roles at BigTech (Google DeepMind, AWS Health AI, NVIDIA BioNemo).

## Files

| File | Purpose |
|------|---------|
| `MahaswetaBhattacharya_Resume.tex` | LaTeX source — compile on Overleaf or any TeX distribution to produce the PDF |
| `MahaswetaBhattacharya_Resume.md`  | Markdown version — paste into Word / Google Docs |
| `MahaswetaBhattacharya_Resume.txt` | Plain-text version — guaranteed-clean copy for ATS upload (Greenhouse, Workday, iCIMS) |

## How to compile the LaTeX → PDF

### Option 1 — Overleaf (easiest)
1. Sign in at <https://www.overleaf.com>.
2. New Project → Upload Project → drag in `MahaswetaBhattacharya_Resume.tex`.
3. Set the compiler to **pdfLaTeX** (default).
4. Click **Recompile**, then **Download PDF**.

### Option 2 — Local
```bash
pdflatex MahaswetaBhattacharya_Resume.tex
```

## How to update the live site PDF

After regenerating the PDF, replace the file the website serves:

```bash
cp MahaswetaBhattacharya_Resume.pdf ../assets/MahaswetaBhattacharya_Resume.pdf
git add ../assets/MahaswetaBhattacharya_Resume.pdf resume/
git commit -m "Update resume: polished BigTech AI/ML Scientist version"
git push origin main
```

The website's "Download CV" buttons (in `index.html` and `/resume/`) already point to `/assets/MahaswetaBhattacharya_Resume.pdf`, so they'll serve the new file automatically.

