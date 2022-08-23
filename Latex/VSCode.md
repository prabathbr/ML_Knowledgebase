Ref : 

https://aumisb.github.io/2019/06/09/visual-studio-code-for-tex.html

latex-workshop.latex.recipe.default -> lastUSed

VSCode Settings : CTRL + SHIFT + P

Receipe use : latexmk (xelatex)

% !TEX program = xelatex
% !TeX TXS-program:bibliography = txs:///biber

% Referencing Style
\usepackage[
backend=biber,
style=ieee,
url=false,
isbn=false,
doi=false,
]{biblatex}
\addbibresource{refer.bib} %Imports bibliography file


%Clear unwanted items from references
\AtEveryBibitem{
  \clearfield{note}
  \clearfield{pages}
}



\printbibliography
