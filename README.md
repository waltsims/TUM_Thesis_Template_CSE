# CSE Thesis Template
## Background

This template is built upon one provided by the CSE chair @TUM in 2016. Though
I am not firmiliar with the origional owner, I owe them much of the credit for
this work.  The origional publisher of this document for CSE was Yoshiyuki Sakai. 

## Dependencies

- [install](https://www.latex-tutorial.com/installation/) LaTeX
- install [Pygments](http://pygments.org) for
  [minted](ftp://ftp.dante.de/tex-archive/macros/latex/contrib/minted/minted.pdf)

Note: if you prefer not to use minted (due to useability or preference), the
package can of course be removed by commenting 
[these lines of code](https://github.com/waltsims/Thesis_Template_CSE/blob/master/components/settings.tex#L41-L48)
 with a \% symbol
and removing the minted example 
[here](https://github.com/waltsims/Thesis_Template_CSE/blob/master/chapters/Introduction.tex#L51-L82).
The listings package can be used by uncommmenting 
[here](https://github.com/waltsims/Thesis_Template_CSE/blob/master/components/settings.tex#L40).

 
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

**Note for IDE:** If you are using an IDE, you may be able to specify the `-shell-escape`
flag in its settings or to specify an option specific to your builder in the `main.tex`
file. For example, this is known to work for the latex-tools package for Atom and Sublime:

   `% !TEX option = -shell-escape`

## Getting Started with LaTeX
 A great resource for learning LaTeX can be found
[here](https://tobi.oetiker.ch/lshort/lshort.pdf)
and is a great starting point for beginners.

