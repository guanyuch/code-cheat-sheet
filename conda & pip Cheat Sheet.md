## Auto Environment Setting
### check the setting:
conda config --show | grep auto_activate_base
### set it to false:
conda config --set auto_activate_base False <br />
source ~/.bashrc
### set it to true:
conda config --set auto_activate_base True <br />
source ~/.bashrc
