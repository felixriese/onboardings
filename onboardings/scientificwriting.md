# Scientific Writing

## Articles with LaTeX

We highly recommend writing scientific articles with LaTeX.
You can [download](https://www.latex-project.org/get/) LaTeX for free on every operating system.

**Editor:**

* For Mac, we recommend Texpad.
* For every operating system in combination with internet access, Overleaf is a nice online tool. You save time to set up your LaTeX environment and get a lot of free templates.

**Templates:**

- For a Bachelor thesis, Master thesis or PhD thesis, one good template is the [cleanthesis](http://cleanthesis.der-ric.de) template.
- Also, check out the [Overleaf](https://de.overleaf.com/latex/templates) templates.


**Tables:**

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

For multirow and multicolumn support, check out the `multirow` package.

**Multiple figures at once:**

```latex
% \usepackage{subfig}

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

## Posters

Until this year (2020), most scientific posters are overloaded with content.
One great example is [#betterposter](https://www.youtube.com/watch?v=1RwJbhkCA58).
A collection of AI posters can be found here: [postersession.ai](https://postersession.ai).

## Scientific Plots

* Colormaps: Use *viridis*, never use jet/rainbow. Learn why [here](https://cran.r-project.org/web/packages/viridis/vignettes/intro-to-viridis.html) or in this ([video](https://www.youtube.com/watch?v=xAoljeRJ3lU)).
