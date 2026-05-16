# PHT3D Course Guide

LaTeX source for the PHT3D reactive transport modelling short course guide.

## Contents

The guide covers:
- Physical transport (1D/2D advection-dispersion)
- Geochemical equilibrium and mineral reactions
- Reactive transport coupling
- Ion exchange
- Surface complexation modelling (SCM)
- Redox reactions
- Kinetics (commented out by default — enable as needed)

## Building the PDF

```bash
pdflatex course_guide.tex
bibtex course_guide
pdflatex course_guide.tex
pdflatex course_guide.tex
```

## Customising for a new course

1. Edit `titlepage.tex` — update `\maintitle`, `\subtitle` (venue/dates), and the instructor list.
2. Enable or disable chapters in `course_guide.tex` by commenting/uncommenting `\include{...}` lines.
3. Compile as above.
