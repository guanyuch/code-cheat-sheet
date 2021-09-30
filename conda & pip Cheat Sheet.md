# **conda & pip Cheat Sheet**

## **1. conda**

#### Verify conda is installed, check version number
- `conda info `

#### Update conda to the current version
- `conda update conda `

#### Install a package included in Anaconda
- `conda install PACKAGE NAME `

#### Install a package (scikit-learn) from a specific channel (conda-forge)
- `conda install --channel conda-forge scikit-learn `

#### Update an installed program
- `conda update PACKAGE NAME `

#### Remove one or more packages (scikit-learn, numpy) from a specific environment (py38)
- `conda remove --name py38 scikit-learn numpy `

#### Search for a package
- `conda search PACKAGE NAME `

#### Get a list of all my environments, active environment is shown with *
- `conda env list `

#### Create a new environment named py38, install Python 3.8
- `conda create --name py38 python=3.8 `

#### Make exact copy of an environment
- `conda create --clone py38 --name py38-2 `

#### Activate the new environment to use it
- WINDOWS: ` activate py38 `
- LINUX, macOS: ` source activate py38 `

#### Deactivate the new environment to use it
- WINDOWS: ` deactivate py38 `
- LINUX, macOS: ` source deactivate py38 `

#### Auto Environment Setting
#### Check the setting
- `conda config --show | grep auto_activate_base `
#### Set it to false
- `conda config --set auto_activate_base False `
#### Set it to true
- `conda config --set auto_activate_base True `

## **2. pip**

#### Install a package directly from PyPI into the current environment using pip
- `pip install scikit-learn `

#### Then add and commit
- `git add FILE NAME`
- `git status`
- `git commit -m "first small text field" -m "optional extended description"`

#### Create new repo on Github for this local file
(Create new repo on Github, then use below code to connect)
- `git remote add origin GITHUB SSH LINK`

#### Check the connection
- `git remote -v`

#### Push it to GitHub
- `git push -U ORIGIN MASTER`

## **3. Git branch**

#### Check all branches
- `git branch` <br />
(* marks the branch you are on)

#### Create new branch
- `git checkout -b BRANCH NAME`

#### Change to a new branch
- `git checkout BRANCH NAME`

#### Check file changes comparing to another branch
- `git diff BRANCH NAME 2`

#### Push to GitHub
- `git push -u origin BRANCH NAME`

#### Pull request from master branch to merge feature branch
- `git pull origin BRANCH NAME`

#### Delete merged branch
- `git branch -d BRANCH NAME`
