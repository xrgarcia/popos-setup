# popos-setup
This is how i setup my popos linux laptop for development...

Pop os version 22 uses python 3.10 as the default. If you try and remove it, you will have to rebuild the box :-(.

# My First goal is to get pipenv working.
sudo apt install pip3
pip --version
pip install pipenv

# add pipenv install dir to .bashrc 

# create a test python project
# NOTE: current version of pipenv 
mkdir ~/code/test/test-pipenv-proj
cd ~/code/test/test-pipenv-proj
SETUPTOOLS_USE_DISTUTILS=stdlib pipenv install # https://github.com/microsoft/WSL/issues/8327
