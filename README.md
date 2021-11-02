## 2.2.3 Take Detailed Notes
We highly recommend keeping a journal of:
- All the commands typed in at the command line, and their results
- What is installed via GUI installers

# Conda

Miniconda is a free minimal installer for conda. It is a small,
bootstrap version of Anaconda that includes only conda, Python, the
packages they depend on, and a small number of other useful packages,
including pip, zlib and a few others. Use the conda install command to
install 720+ additional conda packages from the Anaconda repository.

# PostgresSQL

`$ sudo apt install postgresql-client`

`$ sudo apt install postgresql`

`$ ss -nlt` : "Once PostgreSQL Server has finished installing, you should be able to see it listening for incoming connections on port 5432. This is a good way to confirm that it’s up and running as expected."

# Virtualenv

Install pyenv on Ubuntu:

```
#!/bin/bash

sudo apt-get install git python-pip make build-essential libssl-dev zlib1g-dev libbz2-dev libreadline-dev libsqlite3-dev curl
sudo pip install virtualenvwrapper

git clone https://github.com/yyuu/pyenv.git ~/.pyenv
git clone https://github.com/yyuu/pyenv-virtualenvwrapper.git ~/.pyenv/plugins/pyenv-virtualenvwrapper

echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.bashrc
echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(pyenv init -)"' >> ~/.bashrc
echo 'pyenv virtualenvwrapper' >> ~/.bashrc

exec $SHELL
```