# opencv-webapp

## Intro

- https://www.cvlecture.marearts.com/
- http://www.marearts.com/webapp/dface/

**What do we need?**

- Django Web Framework
- Linux (Windows or Mac is also ok)
- Python
- Python-OpenCV

**Video information**

- linux, python3, pip3 install - https://youtu.be/gVarJ1DRhow

- virtualenv install -  https://youtu.be/LPzJBPpzL4I 

- opencv + python install - https://youtu.be/Ji1LsVZZYCA 

- django install - https://youtu.be/gAlraBTmQ3Y

**Ubuntu Linux install**

1. Virtual machine

- VirtualBox : https://www.virtualbox.org
- VMware : https://www.vmware.com
- parallels : https://www.parallels.com/eu/

2. Ubuntu : https://www.ubuntu.com/download/desktop

3. VirtualBox + Ubuntu install

- https://www.lifewire.com/run-ubuntu-within-windows-virtualbox-2202098 (English)
- http://blog.happydong.kr/252

**Django & OpenCV install**

1. Python 3.6 & pip3

python 3.6 install

```
$sudo add-apt-repository ppa:jonathonf/python-3.6
$sudo apt-get update
$sudo apt-get install python3.6
```

pip3 install

```
$wget https://bootstrap.pypa.io/get-pip.py
$sudo python3.6 get-pip.py
$sudo ln -s /usr/bin/python3.6 /usr/local/bin/python3 #terminal reopen
```

version check

```
$python --version  # (this will reflect your choice, see above)
$python3 --version
$pip --version
$pip3 --version
```

Old

```
$(head -1 `which pip` | tail -c +3) --version
$(head -1 `which pip3` | tail -c +3) --version
```

2. Virtualenv wrapper

virtualenvwrapper install

```
$sudo -H pip3 install virtualenvwrapper
edit .bashrc
$which python3.6 
/usr/bin/python3.6
```

```
$nano ~/.bashrc #add below sentence
VIRTUALENVWRAPPER_PYTHON='<Python3 location>'
source /usr/local/bin/virtualenvwrapper.sh
export WORKON_HOME=$HOME/.virtualenvs
```

```
$mkdir ~/.virtualenvs
$source ~/.bashrc
```

make virtual environment

```
$ mkvirtualenv envpy3 #<project name>
$(envpy3) python3 -m pip install --upgrade pip
```

3. OpenCV-python

opencv-python install

```
$(envpy3)python3 -m pip install opencv-python
!! (It is wrong) -> pip install opencv-python (X)
```

PyCharm install
PyCharm community : https://www.jetbrains.com/pycharm/download
 - install
 - interpreter setting
 - opencv face detection test 
   : https://github.com/MareArts/cvlecture_opencv-webapp/tree/master/face_detection

4. Django

Django install

```
$(envpy3) pip install django
```

make project

```
$(envpy3)django-admin startproject opencv_webapp .
```

run on terminal

```
$(envpy3)python manage.py runserver 127.0.0.1:8000
```

run on pycharm
 - open project
 - setting interpreter
 - run
 

Reference for Django 
Django girls 
https://tutorial.djangogirls.org/en/installation/ (english),
https://tutorial.djangogirls.org/ko/installation/ (한글)

Reference
opencv face detection source code : https://github.com/MareArts/cvlecture_opencv-webapp/tree/master/face_detection


## Preparation

## Django

## Website Publish

## Face & Eye Detection Webapp

## References

- https://www.udemy.com/opencv-webapp/learn/v4/t/lecture/10801668?start=0
