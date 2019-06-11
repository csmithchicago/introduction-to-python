# Learning Python through Jupyter Notebooks

## Installation

To work through these notebooks you will first need to have both python3 and git installed.


We will use miniconda as our python installation. Miniconda is a reduced version of anaconda that comes with fewer packages installed globally. Since we will be using virtual environments we don't install packages globally but rather they are installed locally for every virtual environment on our machine. To download miniconda, follow the instructions [here](https://docs.conda.io/en/latest/miniconda.html) to download python 3.7 for your system. Instructions for installing git can be found [here](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).

### Virtual Environment

To help with organization of packages and to avoid conflict with any system versions of python that might be pre-installed on your operating system, we use virtual environments to isolate our project. This also makes it easier for packaging code that needs to be used in multiple environments.

From the command line we create a virtual environment called `my-project` in the home directory using the following command.

`username:~$ python3 -m venv my-project`

Now we move into the new folder and clone the repository to create local copies of theses notebooks.

`username:~$ cd my-project`
`username:~/my-project$ git clone https://github.com/csmithchicago/introduction-notebooks`

We can now activate the virtual environment and install the packages needed for running the notebooks.

`username:~/my-project$ source bin/activate`
`(my-project) username:~/my-project$ cd introduction-notebooks`
`(my-project) username:~/my-project/introduction-notebooks$ pip install -r requirements.txt`

After activation of the virtual environment you will see the name of the environment you are in displayed at the beginning of the bash prompt. To exit a virtual environment run `deactivate` from the command line.

## Command Line Tools

| Notebook | Description |
|--------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [linux](http://nbviewer.ipython.org/github/donnemartin/data-science-ipython-notebooks/blob/master/commands/linux.ipynb) | Unix-like and mostly POSIX-compliant computer operating system.  Disk usage, splitting files, grep, sed, curl, viewing running processes, terminal syntax highlighting, and Vim.|
| [git](http://nbviewer.ipython.org/github/donnemartin/data-science-ipython-notebooks/blob/master/commands/misc.ipynb#git) | Distributed revision control system with an emphasis on speed, data integrity, and support for distributed, non-linear workflows. |
| [ipython notebook](http://nbviewer.ipython.org/github/donnemartin/data-science-ipython-notebooks/blob/master/commands/misc.ipynb#ipython-notebook) | Web-based interactive computational environment where you can combine code execution, text, mathematics, plots and rich media into a single document. |

## Basic Python

| Notebook | Description |
|-----------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|
| [data structures](http://nbviewer.ipython.org/github/donnemartin/data-science-ipython-notebooks/blob/master/python-data/structs.ipynb) | Learn Python basics with tuples, lists, dicts, sets. |
| [data structure utilities](http://nbviewer.ipython.org/github/donnemartin/data-science-ipython-notebooks/blob/master/python-data/structs_utils.ipynb) | Learn Python operations such as slice, range, xrange, bisect, sort, sorted, reversed, enumerate, zip, list comprehensions. |
| [functions](http://nbviewer.ipython.org/github/donnemartin/data-science-ipython-notebooks/blob/master/python-data/functions.ipynb) | Learn about more advanced Python features: Functions as objects, lambda functions, closures, *args, ** kwargs currying, generators, generator expressions, itertools. |
| [logging](http://nbviewer.ipython.org/github/donnemartin/data-science-ipython-notebooks/blob/master/python-data/logs.ipynb) | Learn about Python logging with RotatingFileHandler and TimedRotatingFileHandler. |
| [pdb](http://nbviewer.ipython.org/github/donnemartin/data-science-ipython-notebooks/blob/master/python-data/pdb.ipynb) | Learn how to debug in Python with the interactive source code debugger. |


## Numpy

IPython Notebook(s) demonstrating NumPy functionality.

| Notebook | Description |
|--------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [numpy](http://nbviewer.ipython.org/github/donnemartin/data-science-ipython-notebooks/blob/master/numpy/numpy.ipynb) | Adds Python support for large, multi-dimensional arrays and matrices, along with a large library of high-level mathematical functions to operate on these arrays. |
| [Introduction-to-NumPy](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/numpy/02.00-Introduction-to-NumPy.ipynb) | Introduction to NumPy. |
| [Understanding-Data-Types](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/numpy/02.01-Understanding-Data-Types.ipynb) | Learn about data types in Python. |
| [The-Basics-Of-NumPy-Arrays](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/numpy/02.02-The-Basics-Of-NumPy-Arrays.ipynb) | Learn about the basics of NumPy arrays. |
| [Computation-on-arrays-ufuncs](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/numpy/02.03-Computation-on-arrays-ufuncs.ipynb) | Learn about computations on NumPy arrays: universal functions. |
| [Computation-on-arrays-aggregates](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/numpy/02.04-Computation-on-arrays-aggregates.ipynb) | Learn about aggregations: min, max, and everything in between in NumPy. |
| [Computation-on-arrays-broadcasting](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/numpy/02.05-Computation-on-arrays-broadcasting.ipynb) | Learn about computation on arrays: broadcasting in NumPy. |
| [Boolean-Arrays-and-Masks](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/numpy/02.06-Boolean-Arrays-and-Masks.ipynb) | Learn about comparisons, masks, and boolean logic in NumPy. |
| [Fancy-Indexing](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/numpy/02.07-Fancy-Indexing.ipynb) | Learn about fancy indexing in NumPy. |
| [Sorting](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/numpy/02.08-Sorting.ipynb) | Learn about sorting arrays in NumPy. |
| [Structured-Data-NumPy](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/numpy/02.09-Structured-Data-NumPy.ipynb) | Learn about structured data: NumPy's structured arrays. |



## Pandas

IPython Notebook(s) demonstrating pandas functionality.

| Notebook | Description |
|--------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [pandas](http://nbviewer.ipython.org/github/donnemartin/data-science-ipython-notebooks/blob/master/pandas/pandas.ipynb) | Software library written for data manipulation and analysis in Python. Offers data structures and operations for manipulating numerical tables and time series. |
| [github-data-wrangling](https://github.com/donnemartin/viz/blob/master/githubstats/data_wrangling.ipynb) | Learn how to load, clean, merge, and feature engineer by analyzing GitHub data from the [`Viz`](https://github.com/donnemartin/viz) repo. |
| [Introduction-to-Pandas](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/pandas/03.00-Introduction-to-Pandas.ipynb) | Introduction to Pandas. |
| [Introducing-Pandas-Objects](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/pandas/03.01-Introducing-Pandas-Objects.ipynb) | Learn about Pandas objects. |
| [Data Indexing and Selection](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/pandas/03.02-Data-Indexing-and-Selection.ipynb) | Learn about data indexing and selection in Pandas. |
| [Operations-in-Pandas](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/pandas/03.03-Operations-in-Pandas.ipynb) | Learn about operating on data in Pandas. |
| [Missing-Values](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/pandas/03.04-Missing-Values.ipynb) | Learn about handling missing data in Pandas. |
| [Hierarchical-Indexing](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/pandas/03.05-Hierarchical-Indexing.ipynb) | Learn about hierarchical indexing in Pandas. |
| [Concat-And-Append](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/pandas/03.06-Concat-And-Append.ipynb) | Learn about combining datasets: concat and append in Pandas. |
| [Merge-and-Join](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/pandas/03.07-Merge-and-Join.ipynb) | Learn about combining datasets: merge and join in Pandas. |
| [Aggregation-and-Grouping](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/pandas/03.08-Aggregation-and-Grouping.ipynb) | Learn about aggregation and grouping in Pandas. |
| [Pivot-Tables](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/pandas/03.09-Pivot-Tables.ipynb) | Learn about pivot tables in Pandas. |
| [Working-With-Strings](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/pandas/03.10-Working-With-Strings.ipynb) | Learn about vectorized string operations in Pandas. |


## Matplotlib

| Notebook | Description |
|-----------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------|
| [matplotlib](http://nbviewer.ipython.org/github/donnemartin/data-science-ipython-notebooks/blob/master/matplotlib/matplotlib.ipynb) | Python 2D plotting library which produces publication quality figures in a variety of hardcopy formats and interactive environments across platforms. |
| [matplotlib-applied](http://nbviewer.ipython.org/github/donnemartin/data-science-ipython-notebooks/blob/master/matplotlib/matplotlib-applied.ipynb) | Apply matplotlib visualizations to Kaggle competitions for exploratory data analysis.  Learn how to create bar plots, histograms, subplot2grid, normalized plots, scatter plots, subplots, and kernel density estimation plots. |
| [Introduction-To-Matplotlib](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/matplotlib/04.00-Introduction-To-Matplotlib.ipynb) | Introduction to Matplotlib. |
| [Simple-Line-Plots](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/matplotlib/04.01-Simple-Line-Plots.ipynb) | Learn about simple line plots in Matplotlib. |
| [Simple-Scatter-Plots](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/matplotlib/04.02-Simple-Scatter-Plots.ipynb) | Learn about simple scatter plots in Matplotlib. |
| [Errorbars.ipynb](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/matplotlib/04.03-Errorbars.ipynb) | Learn about visualizing errors in Matplotlib. |
| [Density-and-Contour-Plots](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/matplotlib/04.04-Density-and-Contour-Plots.ipynb) | Learn about density and contour plots in Matplotlib. |
| [Histograms-and-Binnings](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/matplotlib/04.05-Histograms-and-Binnings.ipynb) | Learn about histograms, binnings, and density in Matplotlib. |
| [Customizing-Legends](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/matplotlib/04.06-Customizing-Legends.ipynb) | Learn about customizing plot legends in Matplotlib. |
| [Customizing-Colorbars](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/matplotlib/04.07-Customizing-Colorbars.ipynb) | Learn about customizing colorbars in Matplotlib. |
| [Multiple-Subplots](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/matplotlib/04.08-Multiple-Subplots.ipynb) | Learn about multiple subplots in Matplotlib. |
| [Text-and-Annotation](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/matplotlib/04.09-Text-and-Annotation.ipynb) | Learn about text and annotation in Matplotlib. |
| [Customizing-Ticks](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/matplotlib/04.10-Customizing-Ticks.ipynb) | Learn about customizing ticks in Matplotlib. |
| [Settings-and-Stylesheets](http://nbviewer.jupyter.org/github/donnemartin/data-science-ipython-notebooks/blob/master/matplotlib/04.11-Settings-and-Stylesheets.ipynb) | Learn about customizing Matplotlib: configurations and stylesheets. |


## Credit
* Repository was forked from Donne Martin's [data science ipython notebooks](https://github.com/donnemartin/data-science-ipython-notebooks.git) repository.
