# CSE Thesis Template
## Background

This template is built upon one provided by the CSE chair @TUM in 2016. Though
I am not firmiliar with the origional owner, I owe them much of the credit for
this work.

## Dependencies

- [install](https://www.latex-tutorial.com/installation/) LaTeX
- install [Pygments](http://pygments.org) for
  [minted](ftp://ftp.dante.de/tex-archive/macros/latex/contrib/minted/minted.pdf)
 
## Creating a PDF
creating a PDF from your LaTeX document based on this template consists of
three steps.

1. In the base project directory, run the following command:

   `pdflatex -shell-escape main.tex`.

2. In order to add citations to the work, run:

   `bibtex main`.

3. To recompile with citations repeat step 1.

   `pdflatex -shell-escape main.tex`
 
Your compiled document will be found in the base project directory under
main.pdf.


## Getting Started with LaTeX
 A great resource for learning LaTeX can be found
[here](https://tobi.oetiker.ch/lshort/lshort.pdf)
and is a great starting point for beginners.

