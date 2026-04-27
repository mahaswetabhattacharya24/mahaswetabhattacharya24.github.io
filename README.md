# mahaswetabhattacharya24.github.io

Personal website of Mahasweta Bhattacharya — Senior Scientist (AI/ML) at Sanofi.
Live at https://mahaswetabhattacharya24.github.io

## Two views, same content

| View | URL | Audience |
|---|---|---|
| Visual portfolio | `/` (`index.html`) | General audience, narrative-first, branded look |
| Research portfolio | `/research.html` | Academic / BigTech research recruiters; minimalist al-folio-style |
| Publications | `/publications.html` | Full pub list with BibTeX, abstracts, journal/code links |
| Blog | `/blog.html` | Long-form technical writing on ML for biology, agentic systems, deployment |
| CV / Resume | `/resume/` | Resume in HTML, PDF, LaTeX source, plain-text (ATS) |

The two views are deliberate: the visual site is the "front door" for general visitors,
the research site (`/research.html`) is the format DeepMind / AWS Health / NVIDIA BioNemo
hiring committees expect — clean, text-first, publication-led, with a blog for written
technical signal.

## Files

| Path | Purpose |
|---|---|
| `index.html` | Visual home (single-page narrative portfolio) |
| `research.html` | Research home (minimalist BigTech-style) |
| `publications.html` | Full publications + BibTeX |
| `blog.html` | Blog landing page |
| `blog/posts/*.html` | Individual blog posts |
| `assets/css/research.css` | Shared stylesheet for `/research`, `/publications`, `/blog` |
| `assets/picture.jpg` | Profile photo |
| `assets/MahaswetaBhattacharya_Resume.pdf` | CV PDF (lives on the live site) |
| `resume/` | Resume sources (LaTeX, Markdown, plain text) + `README.md` |
| `about.md`, `projects.md`, `publications.md`, `news.md`, `conferences.md`, `contact.md`, `resume.md` | Jekyll markdown pages backing the visual site |

## Editing the research site

The minimalist style lives in `assets/css/research.css`. All the BigTech-style pages
import it. Light/dark mode is automatic via `prefers-color-scheme`.

To add a blog post:

1. Copy an existing file from `blog/posts/` and rename it `YYYY-MM-DD-slug.html`.
2. Update the `<title>`, `<meta name="description">`, the `<h1>`, the `.post-meta` line, and the body.
3. Add a corresponding entry at the top of the `Posts` section in `blog.html`.

To add a publication:

1. Add a `.pub` block to `publications.html` (with optional `abstract` and `bibtex` divs).
2. Add a short version to the Publications section of `research.html`.
