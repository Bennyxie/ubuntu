1. install
- sudo bash XXXX.sh
- yes
- /usr/local/anaconda3

2. PATH
- export PATH=/usr/local/anaconda3/bin:$PATH


3. Transfer
- conda env export > environment.yml
- conda env create -f environment.yml
