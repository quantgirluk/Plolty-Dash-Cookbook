# Installing Dash and Plotly

Once you have setup your environment, let’s install the `dash` and `plotly` Python libraries.

## Getting ready

For this recipe, we will use the preferred installer program in Python `pip`. So, make sure you have it available in your virtual environment.

Note that starting with Python 3.4, `pip` is included by default into all created virtual environments.

## How to do it

1. You can install `dash` and `plotly` Python  libraries by running the command

```bash
pip install dash
```

This will install the latest versions of both libraries. Alternatively, you can install them one by one by using

```bash
pip install plotly
pip install dash
```

2. Install the `pandas` library by running

```bash
pip install pandas
```

Although `pandas` is not part of the Dash ecosystem, it is required by Plotly Express (a module of `plotly`) and we will use it extensively in our recipes.

3. Verify the installation was successful by running

```bash
pip list
```

This will print a list of all libraries installed in your virtual environment. So, you should be able to see `dash`, `plotly` and `pandas`  in that list.

## How it works

pip is the standard package manager system for Python. It allows you to install and manage packages that are not part of the Python standard library such as Plotly and Dash. By default pip installs packages from the Python Package Index but it also allows you to install them from other indexes, local files, and other sources.

## There’s more

Some useful pip commands

- Uninstall a package

```bash
pip uninstall SomePackage
```

- Install a specific version of a package

```bash
pip install SomePackage==1.0.4
```

- Install a minimum- version of a package

```bash
pip install SomePackage>=1.0.4
```

- Upgrade a package to the latest available

```bash
pip install --upgrade SomePackage
```
