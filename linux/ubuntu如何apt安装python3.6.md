# ubuntu如何安装python3.6

* 首先要增加响应的源，由于该源不存在，所以要安装这个工具
```
apt install software-properties-common
```

* 然后增加Py3.6 ppa
```
sudo add-apt-repository ppa:jonathonf/python-3.6
sudo apt-get update
sudo apt-get install python3.6
apt install python3.6-dev
apt install python3.6-venv
wget https://bootstrap.pypa.io/get-pip.py
python3.6 get-pip.py
pip3.6 install setuptools
```
