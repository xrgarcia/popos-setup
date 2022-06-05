# popos-setup

This is how i setup my popos linux laptop for development...

Pop os version 22 uses python 3.10 as the default. If you try and remove it, you will have to rebuild the box :-(.

## install pyenv to manage python version
So the default 3.10 (at present) has some issues.  Pyenv can/does use shims to ensure the python path(s) goes to something within the users control. highly recommended to install by visiting here https://github.com/pyenv/pyenv#basic-github-checkout=

## get Poetry working
1. Install poetry by visiting https://python-poetry.org/docs/
2. https://github.com/pyenv/pyenv/wiki#suggested-build-environment
3. https://github.com/pyenv/pyenv/wiki/Common-build-problems

## Install Pipenv (DEPRECATED)

```
sudo apt install pip
pip --version
pip install pipenv
```
NOTE: add pipenv install dir to $PATH in .bashrc, something like: export PATH="/path/to/dir:$PATH"

### Setup a pipenv
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

## Improve Battery Life

Reference: https://support.system76.com/articles/battery/
How to add a shell script as an application: https://askubuntu.com/questions/141229/how-to-add-a-shell-script-to-launcher-as-shortcut
