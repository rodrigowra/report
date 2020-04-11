# LaTeX Template Report

* `View`: [main.pdf](https://github.com/rodrigowra/report/blob/master/main.pdf)

* `The report can be downloaded at` : <https://github.com/rodrigowra/report.git>

### Usage

```bash
pdflatex main.tex
bibtex main.tex
pdflatex main.tex
```

### Dependencies

```bash
sudo apt-get install texlive-full
```
LaTeX
-----
<!---
Add the contents of `myfile.tex` into your LaTeX source code, for example using `\input{myfile.tex}`. 
Make sure that the required packages (such as `pgfplots`) are loaded in the preamble of your document as in the example:
-->
```latex
\documentclass[a4paper,11pt]{article}
\input{configs.tex}
\begin{document}
\input{title.tex}
\newpage
\tableofcontents
\thispagestyle{empty}
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
\newpage
\section{Introdução}
\section{Section 1}
\section{Section 2}
\section{Section 3}
\section{Conclusão}
\newpage
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%to insert references
\nocite{ams} 
\addcontentsline{toc}{section}{Referências}
\renewcommand\refname{Referências}
%\bibliographystyle{abntex2-alf}
\bibliographystyle{plain}
\thispagestyle{empty}
\bibliography{referencias}
\thispagestyle{empty}
%\listoftodos
%Example text \todo{Mude aqui} and more text
%\listoftodos[List of suggested changes]
\end{document}
```
<!---*#### Packages

<!---** `amsmath` :Math library
<!---** `amsfonts` : Math Fonts
<!---** `amssymb`: Math Symbols
<!---** `inputenc`: Input of accents, special characters
<!---** `fontenc`: font
<!---** `url`: Use urls
<!---** `hyperref`: destaca links, citações e referências cruzadas,
<!---** `graphicx`: inserção de imagens
<!---** `parskip`: espaço extra entre parágrafos
<!---** `caption`: personaliza o espaço entre a legenda e a figura/fonte
<!---** `microtype`: faz com que o título tenha um espaço maior entre as letras
<!---** `fancyhdr`: cabeçalhos e rodapés
<!---** `titlesec`: personalização dos títulos
<!---** `setspace`: permite aumentar o espaço entre os títulos das seções
<!---** `natbib`: bibliografia
<!---* `geometry`: margens
