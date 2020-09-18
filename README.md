# CV enviroment

## NVIDIA + CUDA + Cudnn


## Python

### Anaconda
- Installation
```
$ wget https://repo.anaconda.com/archive/Anaconda3-2020.07-Linux-x86_64.sh
$ bash Anaconda-xxx.sh
```
- Create a new environment
```
$ conda create -n xbh -y python=3.6
$ conda activate xbh
$ conda install -y ipython pip
$ pip install xxxx
$ conda install pytorch==1.2.0 torchvision==0.4.0 cudatoolkit=9.2 -c pytorch
$ conda deactivate
```
- Remove environment
```
$ rm -rf /path_to_environment
```

### virtualenv
- Installation
```
$ pip install virtualenv
```

- Create a new environment
```
$ virtualenv --python=pythonx.x --no-site-package ./venv
$ source venv/bin/activate
$ pip install xxx
$ deactivate
```

- Remove environment
```
$ rm -rf /path_to_environment
```

### Transfer python package
```
$ pip freeze > requirements.txt
$ pip install -r requirements.txt
```
