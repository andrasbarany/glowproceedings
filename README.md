# GLOW proceedings template

This repository hosts files that you can use to write proceedings for the annual [GLOW colloquium](https://glowlinguistics.org/). [GLOW 47](https://glowlinguistics.org/47/) in Frankfurt am Main is the first to host proceedings.

## What do I need to do?

### Overleaf

If you use [overleaf](https://www.overleaf.com/), you can [create a project](https://www.overleaf.com/latex/templates/glow-proceedings-template/nnzzbmzvfkhm) using the GLOW proceedings template on overleaf. In case you do not have a paid version of overleaf and the project times out, consider [on your own computer](#locally).

### Locally

To use the proceedings template on your own computer, the main file you need is `glow-proceedings-template.tex`. In addition, you should specify some metadata in the preamble of your document. The following shows the preamble of `main.tex` in this repository:

```tex
\input{glow-proceedings-preamble}

% Add your bibliography here
\addbibresource{main.bib}

%% Specify paper metadata ====

% full title of paper
\newcommand{\fulltitle}{GLOW proceedings template}
% short title of paper for header
\newcommand{\shorttitle}{GLOW proceedings template}
% last name of author(s); for multiple use X & Y; X, Y, & Z; X et al.
\newcommand{\authorlast}{Lastname}

%% Specify paper metadata ====

% Specify author(s)
\author{%
    Firstname Lastname \orcidlink{0000-0000-0000-0000}\\
    University of Overleaf\\
    \email{firstname.lastname@overleaf.edu}
}

% Specify your own packages here (keep this to a minimum!)
\usepackage[newfloat]{minted}
\newacronym{wco}{WCO}{weak crossover}

\usepackage{tikz}
\usetikzlibrary{arrows.meta}
\usepackage[linguistics]{forest}
```

Feel free to use `main.tex` and `main.bib` as the basis for your submission. If you compile your file locally, keep in mind that the template uses `fontspec`, so you will need to compile it with XeLaTeX or LuaLaTeX, both of which should be available if your LaTeX installation is recent.

The template also uses `biblatex` (not `natbib`), so compile the bibliography using the `biber` command.

## Getting help

You can open an issue here on github or get in touch via e-mail if you have any questions (abarany _AT_ ed.ac.uk).
