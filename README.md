# Python Handbook

## Table of Contents
1. [Installations](#1-installations)
   - [Anaconda](#11-anaconda)
     - [Installation Guide](#installation-guide)
     - [Open Terminal](#open-terminal)
   - [Visual Studio Code](#12-visual-studio-code)
     - [Installation Guide](#installation-guide-1)
2. [Creating and Activating Conda Environments](#2-creating-and-activating-conda-environments)
   - [Create a Conda Environment](#21-create-a-conda-environment)
   - [Activate the Conda Environment](#22-activate-the-conda-environment)
   - [List Existing Conda Environments](#23-list-existing-conda-environments)
   - [Deactivate the Conda Environment](#24-deactivate-the-conda-environment)
3. [Resources for Further Learning](#3-resources-for-further-learning)

## 1. Installations

### 1.1 Anaconda

Anaconda is a distribution of Python and R for scientific computing and data science. It includes a lot of packages and tools for data science.

#### Installation Guide

Let's first check if it's already installed on your computers:

#### Open Terminal

Open your terminal (or Anaconda Prompt on Windows) to run the following commands to check the installations:

```bash
conda --version
python --version
```

it says that it already exists, use this command in your terminal
```bash
sudo rm -rf /opt/anaconda3
```

1. Go to the [Anaconda website](https://www.anaconda.com/products/distribution).
2. Download the installer for your operating system (Windows, macOS, or Linux).
3. Run the installer and follow the instructions.

**Note for Windows Users:** Make sure to check the option to add Anaconda to your PATH environment during installation.
**Note of Mac Users:** If you are having issues where it says that it already exists, use this command in your terminal
```bash
sudo rm -rf /opt/anaconda3
```

#### Open Terminal

Once Anaconda is installed, open your terminal to run the following commands to check the installations:

```bash
conda --version
python --version
```

Python should already be installed with Anaconda. You can verify the installation using the `python --version` command above.

Jupyter Notebook is included with the Anaconda distribution. To launch Jupyter Notebook, run the following command in your terminal:

```bash
jupyter notebook
```

This will open Jupyter Notebook in your default web browser. We will be using VS code for this tutorial.

### 1.2 Visual Studio Code

Visual Studio Code (VS Code) is a powerful code editor that you can use easily for your data science projects. Another recommended compiler used by professionals is [PyCharm](https://www.jetbrains.com/pycharm/).

#### Installation Guide

1. Go to the [Visual Studio Code website](https://code.visualstudio.com/).
2. Download the installer for your operating system (Windows, macOS, or Linux).
3. Run the installer and follow the instructions.

Once installed, you can open VS Code and start coding!

1. Go to the Extensions view by clicking the square icon in the sidebar or pressing `Ctrl+Shift+X`.
2. Install the Python and Jupyter extensions.
3. From the command palette (`Ctrl+Shift+P`), select `Python: Select Interpreter` and choose the Conda environment.

## 2. Creating and Activating Conda Environments

Creating and using Conda environments is a best practice to manage project-specific dependencies in isolation.

### 2.1 Create a Conda Environment

To create a new Conda environment, use the following command:

```bash
conda create --name myenv
```

Replace `myenv` with the name you want for your environment. You can also specify the Python version and packages:

```bash
conda create --name myenv python=3.11.7 ipython
```

### 2.2 Activate the Conda Environment

To activate the newly created environment, use the command:

```bash
conda activate myenv
```

### 2.3 List Existing Conda Environments

To list existing Conda environments, use the command:

```bash
conda info --envs
```

### 2.4 Deactivate the Conda Environment

When you are done working in the environment, you can deactivate it with:

```bash
conda deactivate
```

## 4. Download BeautifulSoup using Conda:
```bash
conda install -c anaconda beautifulsoup4
from bs4 import BeautifulSoup
```

## 3. Resources for Further Learning

For a whirlwind tour of some of Python's essential syntax and semantics, built-in data types and structures, function definitions, control flow statements, and other aspects of the language, refer to this [Handbook](https://nbviewer.org/github/bagrow/WhirlwindTourOfPython/blob/master/01-Introduction.ipynb).

For additional resources, visit [Further Learning](https://nbviewer.org/github/bagrow/WhirlwindTourOfPython/blob/master/18-Further-Resources.ipynb).

---

This README provides a concise guide to get started with Python, Anaconda, and Visual Studio Code for data science projects.
