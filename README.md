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

## Install pyenv on Ubuntu

1. Install dependencies

```
$ sudo apt-get install -y make build-essential libssl-dev zlib1g-dev libbz2-dev \
libreadline-dev libsqlite3-dev wget curl llvm libncurses5-dev libncursesw5-dev \
xz-utils tk-dev libffi-dev liblzma-dev
```

2. Install pyenv

`$ curl -L https://raw.githubusercontent.com/pyenv/pyenv-installer/master/bin/pyenv-installer | bash`

3. Validate installation

`pyenv -v`

4. If it doesn't show up, add this to your `.zshrc`:

```
export PYENV_ROOT="$HOME/.pyenv"
export PATH="$PYENV_ROOT/bin:$PATH"
if command -v pyenv 1>/dev/null 2>&1; then
 eval "$(pyenv init -)"
fi
```

reference: [](https://bgasparotto.com/install-pyenv-ubuntu-debian) 