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

## Interactive Notebooks

| Notebook | Description |
|-----------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|
| [Data Types](./notebooks/01_Data_Types_in_Python.ipynb) | Learn Python basics with tuples, lists, dicts, sets. |
| [Functions](./notebooks/02_Functions_in_Python.ipynb) | Learn Python operations such as slice, range, xrange, bisect, sort, sorted, reversed, enumerate, zip, list comprehensions. |
| [File I/O](./notebooks/03_File_Input_Output_in_Python.ipynb) | Learn about more advanced Python features: Functions as objects, lambda functions, closures, *args, ** kwargs currying, generators, generator expressions, itertools. |
| [Debugging](./notebooks/04_Debugging_in_Python.ipynb) | Learn about Python logging with RotatingFileHandler and TimedRotatingFileHandler. |
| [more to come](http://nbviewer.ipython.org/github/donnemartin/data-science-ipython-notebooks/blob/master/python-data/pdb.ipynb) | Learn how to debug in Python with the interactive source code debugger. |

## Additional Resources

| Document | Description |
|--------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [Command Line](./documentation/getting_started_with_the_command_line.md) | Unix-like and mostly POSIX-compliant computer operating system.  Disk usage, splitting files, grep, sed, curl, viewing running processes, terminal syntax highlighting, and Vim.|
| [Git (Version Control)](./documentation/getting_started_with_git.md) | Distributed revision control system with an emphasis on speed, data integrity, and support for distributed, non-linear workflows. |
| [Data Analysis](./documentation/getting_started_with_numpy_pandas_matplotlib.md) | Web-based interactive computational environment where you can combine code execution, text, mathematics, plots and rich media into a single document. |

## Bug Reports and Feature Requests

To submit an issue or request a new feature, [submit an issue report](https://github.com/csmithchicago/introduction-to-python/issues) following the provided templates.

### Credit

* Repository initially started as a fork of Donne Martin's [data science iPython notebooks](https://github.com/donnemartin/data-science-ipython-notebooks.git) repository.
