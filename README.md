![](https://github.com/waltsims/TUM_Thesis_Template_CSE/workflows/pdflatex/badge.svg) ![](https://github.com/waltsims/TUM_Thesis_Template_CSE/workflows/xelatex/badge.svg) ![](https://github.com/waltsims/TUM_Thesis_Template_CSE/workflows/lualatex/badge.svg)

# CSE Thesis Template
## Background

This template is built upon one provided by the CSE chair @TUM in 2016. Though
I am not familiar with the original owner, I owe them much of the credit for
this work.  The original publisher of this document for CSE was Yoshiyuki Sakai.

## Other Options

* [From Florian Walch](https://github.com/fwalch/tum-thesis-latex)
* [From Micheal Grupp](https://github.com/MichaelGrupp/TTT)

## Dependencies

- [install](https://www.latex-tutorial.com/installation/) LaTeX
- install [Pygments](http://pygments.org) for
  [minted](ftp://ftp.dante.de/tex-archive/macros/latex/contrib/minted/minted.pdf)

Note: if you prefer not to use minted (due to usability or preference), the
package can of course be removed by commenting
[these lines of code](https://github.com/waltsims/Thesis_Template_CSE/blob/master/components/settings.tex#L98-L104)
 with a \% symbol
and removing the minted example
[here](https://github.com/waltsims/Thesis_Template_CSE/blob/master/chapters/Introduction.tex#L51-L87).
The listings package can be used by uncommenting
[here](https://github.com/waltsims/Thesis_Template_CSE/blob/master/components/settings.tex#L97).


## Creating a PDF
Creating a PDF from your LaTeX document based on this template consists of
three steps.

1. In the base project directory, run the following command:

   `pdflatex -shell-escape main.tex`.

2. In order to add citations to the work, run:

   `bibtex main`.

3. To recompile with citations repeat step 1.

   `pdflatex -shell-escape main.tex`

Your compiled document will be found in the base project directory under
main.pdf.

**Note for IDE:** If you are using an IDE, you may be able to specify the `-shell-escape`
flag in its settings or to specify an option specific to your builder in the `main.tex`
file. For example, this is known to work for the latex-tools package for Atom and Sublime:

   `% !TEX option = -shell-escape`

In case you want to mix more than one languages (e.g. english and german),
using XeLaTeX (instead of LaTeX + Babel) is highly recommended.

## Getting Started with LaTeX
A great resource for learning LaTeX can be found
[here](https://tobi.oetiker.ch/lshort/lshort.pdf)
and is a great starting point for beginners.

## Contribution guide

The idea of this project is to help all students of the TUM during the challenging time of their master's thesis. To this end please give back to the project by contributing features and changes you think can help others. To do so simply open a merge request.
