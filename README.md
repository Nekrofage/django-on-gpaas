Django on PaaS
==============

* Requirements

Instance Simple Hosting:
Python: 3.7
Django: 2.2.4


* Procedure


```
1/ Create the application directory.

sam@sam:~$ mkdir -p PYTHON/MONAPP

sam@sam:~$ cd PYTHON/MONAPP/
sam@sam:~/PYTHON/MONAPP$


2/ Clone the template of a Django application.

sam@sam:~/PYTHON/MONAPP$ git clone https://github.com/Nekrofage/django-on-gpaas.git default

sam@sam:~/PYTHON/MONAPP$ cd default/
sam@sam:~/PYTHON/MONAPP/default$


3/ Add the git remote repository.

sam@sam:~/PYTHON/MONAPP/default$ git remote add gandi git+ssh://{instance_id}@git.{datacenter_id}.gpaas.net/default.git


4/ Push the code to the git remote repository. 

sam@sam:~/PYTHON/MONAPP/default$ git push gandi master


5/ Deploy the application to the default directory.

sam@sam:~/PYTHON/MONAPP/default$ ssh {instance_id}@git.{datacenter_id}.gpaas.net deploy default.git


6/ Use the test url.

http://abcd1234.testmyurl.ws/
```
