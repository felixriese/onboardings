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

## Python for Machine Learning

See [scikit-learn](scikitlearn.md) and [Tensorflow.Keras](keras.md).

## Jupyter Notebooks

*Work in Progress*

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
