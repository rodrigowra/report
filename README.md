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
\nocite{Allen} 

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
