# Onboarding to Python 3

## Python 3 Tutorials

*Work in Progress*

## Style Guides

Style tipps Python:

* [PEP8](https://www.python.org/dev/peps/pep-0008/) style guide
* [Docstring conventions](https://www.python.org/dev/peps/pep-0257/), especially for functions
* Style guide by [Google](https://google.github.io/styleguide/pyguide.html), [Khan](https://github.com/Khan/style-guides/blob/master/style/python.md), [Best Practises](https://gist.github.com/sloria/7001839#the-best-of-the-best-practices-bobp-guide-for-python)

Use linter to ensure code quality and style. Recommendations:

* [pylint](https://github.com/PyCQA/pylint/)

## Packages Worth Checking Out

* [Matplotlib](https://matplotlib.org/tutorials/index.html) and
  [Seaborn](https://seaborn.pydata.org/tutorial.html) for Plots
* [Numpy](https://numpy.org/devdocs/user/quickstart.html) for efficient
  scientific computing
* [Pandas](https://www.datacamp.com/community/tutorials/pandas-tutorial-dataframe-python)
  for Easy-to-Use Data Handling and Data Mining
* Measure and visualize runtime of a python script: [install snakeviz via `pip3 install snakeviz`]

```bash
python3 -m cProfile -o NameOfProfileFile.prof script.py

snakeviz cprofile_test
```

## Python for Machine Learning

See [scikit-learn](scikitlearn.md) and [Tensorflow.Keras](keras.md).

## Jupyter Notebooks

*Work in Progress*

### Magic commands

Magic command for inline plots:

```python3
%matplotlib inline
````

Magic command for retina plots:

```python3
%config InlineBackend.figure_format = 'retina'
````

Auto-load changed packages:

```python3
%load_ext autoreload
%autoreload 2
```

### Print notebooks with RISE

Use [Jupyter Notebooks](http://jupyter.org) with [RISE](https://github.com/damianavila/RISE) for presentations that include code.

1. Enable RISE:

  ```bash
  jupyter-nbextension install rise --py --sys-prefix
  jupyter-nbextension enable rise --py --sys-prefix
  ```

2. Print with RISE:

  * To print the notebook, execute the following commands:

    `jupyter nbconvert --to pdf "MyNotebook.ipynb" --post serve`

  * To print the notebook as slides, the (currently…) best way to do this, is:

    `jupyter nbconvert --to slides "MyNotebook.ipynb" --post serve`

    and to then add *?print-pdf* to the opened html-file that the URL ends with *...MyNotebook.slides.html?print-pdf*.

  * Print this webpage in Chrome with Cmd-P, change layout to landscape, margins = None
