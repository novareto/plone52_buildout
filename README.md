# plone52_buildout

Installationsprozedur für die Plone-Installationen der SIGUV-Kooperation

Installation
============

Vorbereitung des Ubuntu-Systems
-------------------------------

* sudo apt-get install build-essential python-dev libjpeg-dev libxslt-dev supervisor
* sudo apt-get install libpython3-dev
* sudo apt-get install python3-pip
* sudo apt-get install mongodb

Installation von Python-Add-Ons auf dem Server
----------------------------------------------

* pip3 install virtualenv

Vorbereitung und Durchführung des Plone-Buildouts
-------------------------------------------------

* ~ > git clone https://github.com/novareto/plone52_buildout.git $projectname
* ~ > cd $projectname
* ~/$projectname > virtualenv .
* ~/$projectname > ./bin/pip install -r requirements.txt
* ~/$projectname > ./bin/buildout -c develop.cfg

