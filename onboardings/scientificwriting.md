# Scientific Writing

## Articles with LaTeX

We highly recommend writing scientific articles with LaTeX.
You can [download](https://www.latex-project.org/get/) LaTeX for free on every operating system.

### IDEs

* For Mac, we recommend Texpad.
* For every operating system in combination with internet access, Overleaf is a nice online tool. You save time to set up your LaTeX environment and get a lot of free templates.

### Templates

- For a Bachelor thesis, Master thesis or PhD thesis, one good template is the [cleanthesis](http://cleanthesis.der-ric.de) template.
- Also, check out the [Overleaf](https://de.overleaf.com/latex/templates) templates.


### Tables

We recommend to use booktabs as shown in the example below:

```latex
\usepackage{booktabs}

\begin{document}
\begin{table}[htb]
	\caption{Liste von Werkstoffen}
	\begin{tabular}{lcc}
	\toprule

	\end{tabular}
\end{table}
\end{document}
```

For multirow and multicolumn support, check out the `multirow` package:

```latex
\usepackage{multirow}
```

### Figures

For multiple figures at once, you can use the following code snippets:

```latex
% in the header:
\usepackage{subfig}

% in the document:

% with width ratios:
\begin{figure}[tb]
	\centering
	\subfloat[]{\includegraphics[width=0.22\textwidth]{figures/image1.pdf}\label{fig:im1}}\qquad
	\subfloat[]{\includegraphics[width=0.336\textwidth]{figures/image2.pdf}\label{fig:im2}}
	\caption{(a)~blabla (b)~blabla\label{fig:im_all}}
\end{figure}

% with absolute (and same!) heights:
\begin{figure}[tb]
	\centering
	\subfloat[]{\includegraphics[height=4cm, keepaspectratio]{figures/image1.pdf}\label{fig:im1}}\qquad
	\subfloat[]{\includegraphics[height=4cm, keepaspectratio]{figures/image2.pdf}\label{fig:im2}}
	\caption{(a)~blabla (b)~blabla\label{fig:im_all}}
\end{figure}
```

### References

Usually, you can reference figures, tables and more as follows:

```latex
... see Figure~\ref{fig:abc}
```

With the `cleveref` package, you can reference more efficiently and more consistently:

```latex
% in the header:
\usepackage[nameinlink]{cleveref}

% in the document:
... see \Cref{fig:abc}
```

### Units and Numbers

To typeset units and figures correctly, we highly recommend to use the
`siunitx` package:

```latex
% header:
\usepackage{siunitx}
\sisetup{
	separate-uncertainty=true,	% for uncertainties
	binary-units=true,			% GB for Gigabyte
	tophrase={~to~},			% for \SIrange
	detect-weight=true,		    % for bold font in tables
	detect-inline-weight=math,  % for bold font in tables
	detect-all,
}
% additionally for bold font in tables:
\usepackage{etoolbox}
\robustify\bfseries

% document:
\SI{25}{\square\kilo\meter}
```

To use this package for tables, simply change the column type from l/c/r to `S`.

## Posters

Until this year (2020), most scientific posters are overloaded with content.
One great example is [#betterposter](https://www.youtube.com/watch?v=1RwJbhkCA58).
A collection of AI posters can be found here: [postersession.ai](https://postersession.ai).

## Scientific Plots

* Colormaps: Use *viridis*, never use jet/rainbow. Learn why [here](https://cran.r-project.org/web/packages/viridis/vignettes/intro-to-viridis.html) or in this ([video](https://www.youtube.com/watch?v=xAoljeRJ3lU)).
