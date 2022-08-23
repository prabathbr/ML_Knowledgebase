Install :  (https://www.youtube.com/watch?v=4lyHIQl4VM8)  

1. VSCode  
2. MikTex and update as admin from console  
3. Add VSCode addon LaTeX-Workshop  
4. Perl (https://strawberryperl.com/)  

Reference : 

https://aumisb.github.io/2019/06/09/visual-studio-code-for-tex.html

https://github.com/James-Yu/LaTeX-Workshop/wiki/Compile#latex-workshoplatexrecipedefault

latex-workshop.latex.recipe.default -> lastUsed   

latex-workshop.latex.autoBuild.run -> onFileChange

VSCode Settings : CTRL + SHIFT + P

Receipe use : latexmk (xelatex)

```
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

```
