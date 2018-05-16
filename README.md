# python-virtualenv
## virtualenv
`virtualenv` is a tool to create isolated Python environments.
https://pypi.org/project/virtualenv/#description

## virtualenvwrapper
`virtualenvwrapper` is a set of extensions to Ian Bicking’s virtualenv tool. The extensions include wrappers for creating and deleting virtual environments and otherwise managing your development workflow, making it easier to work on more than one project at a time without introducing conflicts in their dependencies.
https://virtualenvwrapper.readthedocs.io/en/latest/

## Installation
```
sudo apt update
sudo apt dist-upgrade
sudo apt install python-pip
sudo apt install virtualenvwrapper
pip install virtualenv
```
Add to ~/.bashrc and all your environments will be stored in ~/virtualenvs.
```
export WORKON_HOME=$HOME/virtualenvs
source /usr/share/virtualenvwrapper/virtualenvwrapper.sh
```
Reload your shell.  
## Create Python3 environment
```
user@host:~$ mkvirtualenv --python=/usr/bin/python3 yourenv
Running virtualenv with interpreter /usr/bin/python3
Using base prefix '/usr'
New python executable in /home/smegol/virtualenvs/yourenv/bin/python3
Also creating executable in /home/smegol/virtualenvs/yourenv/bin/python
Installing setuptools, pip, wheel...done.
(yourenv) user@host:~$
(yourenv) user@host:~$ pip freeze
(yourenv) user@host:~$ python --version
Python 3.6.5
```
## Usage
`lsvirtualenv` - list your environments  
`workon <env_name>` - activate environment  
`deactivate` - deactivate your environment  
`rmvirtualenv <env_name>` - remove environment  

Boom, you done.
