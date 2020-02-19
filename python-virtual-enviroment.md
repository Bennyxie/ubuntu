## Virtualenv
Create a new virtual environment by choosing a Python interpreter and making a `./venv` directory to hold it:
  virtualenv --system-site-packages -p python3 ./venv

Activate the virtual environment using a shell-specific command:
  source ./venv/bin/activate  # sh, bash, ksh, or zsh
 
## Conda
Create a new virtual environment by choosing a Python interpreter and making a `./venv` directory to hold it:
  conda create -n venv pip python=3.7  # select python version

Activate the virtual environment:
  source activate venv
