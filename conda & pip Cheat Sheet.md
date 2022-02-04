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

#### Make the new environment show in Jupyter Notebook kernel list
- ` python -m ipykernel install --user --name py38 --display-name "py38" `

#### Auto Environment Setting
#### Check the setting
- `conda config --show | grep auto_activate_base `
#### Set it to false
- `conda config --set auto_activate_base False `
#### Set it to true
- `conda config --set auto_activate_base True `

#### Save a copy of an environment
- `conda env export > environment.yml `

#### Create an environment from yml
- `conda env create -f environment.yml `

## **2. pip**

#### Install a package directly from PyPI into the current environment
- `pip install scikit-learn `

#### Install a package from a local wheel file
- `pip install PAKCAGENAME.whl `

#### Install specific version
- `pip install requests==2.22.0 `

#### Install packages from a requirements file
- `pip install -r requirements.txt `

#### Uninstall a package
- `pip uninstall scikit-learn `

#### Forcefully upgrade and reinstall a package
- `pip install --upgrade --force-reinstall scikit-learn `

#### Share the List of Dependencies
- `pip freeze > requirements.txt `

#### Install the List of Dependencies
- `pip install -r requirements.txt `
