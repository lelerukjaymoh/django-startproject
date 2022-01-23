# Django startproject

A small shell script to start off you django app development. It rids you the hustle of repeating the same processes everytime you start a django project and gets you django application up and running within two strikes of a button. It automates: 
* Creation of the project folder 
* Creating and activating virtual enviroment
* Updating pip to latest version
* Starting django project *django-admin startproject *
* Starting an app *python manage.py startapp *
* Writing to settings.py, urls.py, views.py, tempalates
* Making migrations and migrating them


## Getting Started

To get started just clone the repo into your machine and get started. The script might not work out of the box, some tweaks and a little bit of hacking :wink: is required as explained in Prerequisites

### Prerequisites

The script works by relying on several bash aliases. 
First to make the script executable from any directory, create a bin directory in your /home folder.

```
~$ mkdir bin
```
Place the djangostartproject script in the */home/USER/bin* folder and then add the path to it in the .bashrc file
Add this line as the end of your .bashrc file **export PATH=$PATH:/home/USER/bin/** USER being the logged in user

Create a .bash_aliases file if you dont have one and add this line **alias djangostart='. djangostartproject'**. 
This is done so that the script can execute a cd command and actually cd into the folder. Not including the **.** and space in the djangostartproject alias will lead to the script not cd*ing* into a directory.

So as to prevent logging out and in again so as to load the changes done to the *.bashrc* run this command from you home directory
```
~$ source ~/.bashrc
``` 

Once that is done you are ready to go.

### Usage
To use the script, cd to anywhere and run **djangostart** followed by the name you would like to give to your project folder.

```
~$ djangostart djangoproject
```
##### Example
![Example of django-startproject](https://github.com/coderjaymoh/django-startproject/blob/master/Peek%202019-10-24%2004-58.gif)

## Contributing
To contribute just make a PR 

