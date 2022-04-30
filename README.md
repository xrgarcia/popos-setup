# popos-setup

This is how i setup my popos linux laptop for development...

Pop os version 22 uses python 3.10 as the default. If you try and remove it, you will have to rebuild the box :-(.

## My First goal is to get pipenv working.

```
sudo apt install pip3
pip --version
pip install pipenv
```
NOTE: add pipenv install dir to $PATH in .bashrc 

## Setup a pipenv
```
mkdir ~/code/test/test-pipenv-proj
cd ~/code/test/test-pipenv-proj
SETUPTOOLS_USE_DISTUTILS=stdlib pipenv install
```
reference: https://github.com/microsoft/WSL/issues/8327


## Setup AWS cli

1. Install the cli tool: https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html
2. Configure Named Profiles: https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-profiles.html

## Install AWS SAM

reference: https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-sam-cli-install-linux.html

## Install Docker

reference: https://linuxhint.com/install-docker-on-pop_os/
run as non root: https://docs.docker.com/engine/install/linux-postinstall/

## Using Git with Multiple AWS Accounts

reference: https://aws.amazon.com/blogs/devops/using-git-with-aws-codecommit-across-multiple-aws-accounts/

## Setup Windows 11 for VirtualBox

I use my pop os linux laptop work work. Windows 11 is necessary for me.  Here is the insturctions for setting up windows 11 in virtualbox: https://lazyadmin.nl/win-11/install-windows-11-in-virtualbox/

