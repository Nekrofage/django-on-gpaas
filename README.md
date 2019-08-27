Django on PaaS
==============

* Requirements

Instance Simple Hosting:
Python: 3.7
Django: 2.2.4


* Procedure

```
sam@sam:~$ mkdir -p PYTHON/MONAPP

sam@sam:~$ cd PYTHON/MONAPP/
sam@sam:~/PYTHON/MONAPP$

sam@sam:~/PYTHON/MONAPP$ git clone https://github.com/Nekrofage/django-on-gpaas.git default

sam@sam:~/PYTHON/MONAPP$ cd default/
sam@sam:~/PYTHON/MONAPP/default$

sam@sam:~/PYTHON/MONAPP/default$ git remote add gandi git+ssh://2120649@git.sd5.gpaas.net/default.git

sam@sam:~/PYTHON/MONAPP/default$ git push gandi master

sam@sam:~/PYTHON/MONAPP/default$ ssh 2120649@git.sd5.gpaas.net deploy default.git

test url: http://84d15b9ca2.testmyurl.ws/
```
