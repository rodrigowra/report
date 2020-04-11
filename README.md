# LaTeX Template Report

* `View`: [Model-Report.pdf](https://github.com/rodrigowra/Report-LaTeX/blob/master/Report.pdf)

* `The report can be downloaded at` : <https://github.com/rodrigowra/Report-LaTeX.git>

### Usage

```bash
pdflatex Model-Report.tex
bibtex Model-Report.tex
pdflatex Model-Report.tex
```

### Dependencies

```bash
sudo apt-get install texlive-full
```
LaTeX
-----
<!---Add the contents of `myfile.tex` into your LaTeX source code, for example using `\input{myfile.tex}`. 
Make sure that the required packages (such as `pgfplots`) are loaded in the preamble of your document as in the example:
-->

```latex
\documentclass{article}

  \usepackage{pgfplots}
  \pgfplotsset{compat=newest}
  %% the following commands are needed for some matlab2tikz features
  \usetikzlibrary{plotmarks}
  \usetikzlibrary{arrows.meta}
  \usepgfplotslibrary{patchplots}
  \usepackage{grffile}
  \usepackage{amsmath}

  %% you may also want the following commands
  %\pgfplotsset{plot coordinates/math parser=false}
  %\newlength\figureheight
  %\newlength\figurewidth

\begin{document}
  \input{myfile.tex}
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
