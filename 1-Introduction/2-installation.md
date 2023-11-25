# Installation
- Install Python & PIP (add to your PATH)
- Use PIP to install Robot Framework
- Use PIP to install SeleniumLibrary (plus any other libraries you want)
- Select & install desired browsers
- Install Selenium Webdrivers for each installed browser
- Install the Pycharm IDE & Intellibot plugin
- Create a base directory to hold all projects


# Python Installation
I've installed the python using miniconda on my Mac Computer.

## Conda
Conda is an open-source package and environment management system that runs on Windows, macOS, and Linux. Conda quickly installs, runs, and updates packages and their dependencies. It also easily creates, saves, loads, and switches between environments on your local computer. It was created for Python programs, but it can package and distribute software for any language.

## Miniconda
Miniconda is a free minimal installer for conda. It is a small bootstrap version of Anaconda that includes only conda, Python, the packages they both depend on, and a small number of other useful packages (like pip, zlib, and a few others). If you need more packages, use the `conda install` command to install from thousands of packages available by default in Anaconda’s public repo, or from other channels, like conda-forge or bioconda.
The first step after installing miniconda is:

```
# check the conda version:
conda --version

# Expected resul
# conda 23.5.2 
```

To create a new python environment, execute the following command:
```
# create a new evoirnment named py312 to install the python 3.12 version
conda create --name py312
```

To list all the existing and newly created environments, run the following command:
```
conda env list
```

```
# Sample result of above command
# conda environments:
#
base                  *  /Users/aghaamil/miniconda3
py312                    /Users/aghaamil/miniconda3/envs/py312
```

To switch to another environment from the list, use the following command:
```
conda activate py312
```

The first requirement for this new environment is to install Python:
```
conda install python=3.12

# check the installed version by:
# python --version
```

To exit the current environment, enter the following command:
```
conda deactivate

# going to the (base) environment by default
```

# Installing Robot Framework
To leave all the conda environments, type the above command in the (base) environment.
The easiest way to use pip is by letting it find and download packages it installs from the [Python Package Index (PyPI)](https://pypi.org/project/robotframework), but it can also install packages downloaded from the PyPI separately. The most common usages are shown below and [pip](https://pip.pypa.io/) documentation has more information and examples.

```
# Install the latest version (does not upgrade)
pip install robotframework

# Upgrade to the latest stable version
pip install --upgrade robotframework

# Uninstall
pip uninstall robotframework
```

[SeleniumLibrary](https://github.com/robotframework/SeleniumLibrary) is a web testing library for [Robot Framework](https://robotframework.org/) that utilizes the [Selenium](https://www.seleniumhq.org/) tool internally. The project is hosted on [GitHub](https://github.com/robotframework/SeleniumLibrary) and downloads can be found from [PyPI](https://pypi.python.org/pypi/robotframework-seleniumlibrary).

To Install required libraries, run the following command:
```
pip install robotframework-seleniumlibrary
```

🏠 `RequestsLibrary` is a [Robot Framework](https://robotframework.org/) library aimed to provide HTTP api testing functionalities by wrapping the well known [Python Requests Library](https://github.com/kennethreitz/requests).


