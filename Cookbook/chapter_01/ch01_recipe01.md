# Setting up your Python environment

This recipe will guide you through setting up a Python environment to kick-start interactive visualizations by creating a dedicated virtual environment. Virtual environments are an essential tool for managing dependencies specific to each project, helping avoid conflicts between packages, as well as ensuring smooth development and reproducibility.

## Getting ready

Make sure you have a Python distribution (preferably 3.10 or higher) in your operating system. You can download it from its [official website](https://www.python.org/downloads/).

In addition, it would be useful to have an IDE. There are many options in the Python space, but we recommend:

- Visual Studio Code
- PyCharm (the Community edition is free and offers great functionality for beginners)
- Jupyter Notebook

## How to do it

1. Create a virtual environment `ven`  to start working

```bash
python3 -m venv venv
```

Note that the second `venv` is the **name** of your new environment. You can choose any other name that you like but `venv` is probably the most common one.

This command will create a directory named `venv` containing the virtual environment in the path from where you are running it. If you want to create it on a different path, you need to specify it by passing the name of the target path after the name of the new environment as follows:

```bash
python3 -m venv /path/to/new/virtual/venv
```

2. Activate your virtual environment by running

- On macOS/Linux

``
$source venv/bin/activatev
``

- On Windows

```bash
# In cmd.exe
venv\Scripts\activate.bat
# In PowerShell
venv\Scripts\Activate.ps1
```

## How it works

**What is a virtual environment and why are we using one?**

- A virtual environment is a semi-isolated Python environment that allows Python users to install and manage packages for use by a particular application or project, rather than being installed system wide. This guarantees that there is no interfering with the behavior of other Python applications running on the same system.
- `venv` is the standard tool for creating virtual environments in Python. It has been part of Python since Python 3.3.

## There’s more

Some IDEs have special functionality to help you create and configure virtual environments. For example:

- [Visual Studio Code - Environments](https://code.visualstudio.com/docs/python/environments)
- [PyCharm - Creating a virtual environment](https://www.jetbrains.com/help/pycharm/creating-virtual-environment.html)

See also

- The official documentation of [venv — Creation of virtual environments](https://docs.python.org/3/library/venv.html)
