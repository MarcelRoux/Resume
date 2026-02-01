# Marcel Roux — Resume & CV (LaTeX)

This repository contains the source files for my **resume** and **extended CV**, authored in LaTeX and compiled locally using XeLaTeX.

The setup allows multiple document variants (e.g. a concise, one-page resume and a more detailed CV) to be generated from a shared structure, ensuring consistency while tailoring depth to context.

---

## Documents

- **Resume**  
  A concise, one-page summary intended for job applications and recruiter screening.

- **CV (Extended)**  
  A more detailed version including expanded role descriptions and technical depth, shared upon request or during later interview stages.

---

## Build Requirements

- **XeLaTeX** (required)
- A standard LaTeX distribution (e.g. **MacTeX**)

The underlying class relies on common LaTeX packages, including (but not limited to):

- `fontspec`
- `geometry`
- `hyperref`
- `longtable`
- `fancyhdr`
- `xcolor`
- `parskip`

---

## Building Locally

From the repository root:

```sh
latexmk -pdf -xelatex main_resume.tex
latexmk -pdf -xelatex main_cv.tex
```

Artifacts can optionally be configured to output to a dedicated directory (e.g. out/).

---

Design Notes
- The resume prioritizes scanability and ATS compatibility.
- The CV prioritizes technical completeness and narrative clarity.
- Hyphenation is disabled globally to avoid PDF text extraction issues.
- GitHub is intentionally shown only in the footer to avoid header clutter.

---

## Template Attribution

This resume is built on top of the Adaptive CV LaTeX class by Alessandro Rossini.
- Original template: https://alessandrorossini.org
- License: LaTeX Project Public License (LPPL) v1.3+

Significant modifications have been made to layout, macros, and styling to suit a senior software engineering resume rather than an academic CV.

---

## License

This repository contains personal resume content.

The underlying LaTeX class (adcv.cls) and language definitions remain under their original LPPL license as noted above.