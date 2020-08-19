# text-analysis-workshop

Learnings from Bay-SICSS 2020


[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/MindyChang/text-analysis-workshop/master?filepath=index.ipynb)

Direct link:
https://mybinder.org/v2/gh/MindyChang/text-analysis-workshop/master?filepath=index.ipynb


# Installation on Mac
In order to use Jupyter notebooks locally on your own computer:

## Install R

Download and install R from https://cloud.r-project.org/


## Install Python

1. Install Xcode, Apple's developer tools
from https://apps.apple.com/us/app/xcode/id497799835?ls=1&mt=12

2. Install brew, a program that helps you install other programming tools

`/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`

3. Install git

`brew install git`

4. Install Python scripting language

`brew install python3`



## Download this repository
Clone this repo using

`git clone https://github.com/MindyChang/text-analysis-workshop`


## Install Jupyter Notebook
```
pip install notebook
```

#### Install "Table of Contents" Extension:

https://jupyter-contrib-nbextensions.readthedocs.io/en/latest/nbextensions/toc2/README.html

```
pip install jupyter_contrib_nbextensions
jupyter contrib nbextension install --user
jupyter nbextension enable toc2/main
```

If you run into version conflict issues for package X, you can try

```
pip install --upgrade X
```
## Configure Jupyter for R
Open the R console by typing `r` in the terminal and paste the following commands.

Install packages
```
install.packages(c(
'repr',
'IRdisplay',
'evaluate',
'crayon',
'pbdZMQ',
'devtools',
'uuid',
'digest',
'git2r'
), dependencies = TRUE)
```
Install and make the R kernel visible to Jupyter
```
devtools::install_github('IRkernel/IRkernel')
IRkernel::installspec(user = FALSE)
```
## Usage

### Run and code interactively

To run Jupyter notebook interactively, in the terminal, go to the directory where you've downloaded the notebook.

```
jupyter notebook
```

You will be directed to the browser and can then choose and interact with the notebook.
