https://www.youtube.com/watch?v=b4iFyrLQQh4i

1). Project Asset Settings
a). Theme selection
https://demo.w3layouts.com/demos_new/template_demo/07-03-2020/estate_liberty-demo_Free/58112989/web/index.html
b). or other template resources
https://preview.colorlib.com/#konato
C). Lightbox CSS
https://lokeshdhakar.com/projects/lightbox2/

2). Create project folder
3). pyenv local python-version
4). mkvirtualenv project-name // better use project-name as the environment name
5). workon project-name // Switch to the project environment
6). pip freeze // check any package installed
7). pip list // show all package with version information
8). pip show django // show django version
9). pip install django==version // install django inside the virtualenv folder

## Build the main project folder

10). django-admin startproject name // create a main project folder then control job will pass the manage.py
11). after manage.py show up then switch to python manage for the main control command
12). in vscode, command+p, select interpreter, pick the virtual name
13). install pep8 for VS code

## Git setup

14). git init // setup git by creating .gitignore
15). goto gitignore.io, pick the framework for ignore
16). git init // setup .git folder
17). git add . && git commit -m "Initial commit"
18). python manage.py runserver
a). go to localhost:8000, if the page is up then the inital setup is correct
19). once the server is running, db.sqlite3 created. this is not the db for real application
20). within btre folder, settings.py is the important one
a). within settings, allowed hosts [] is for server deployment, server provide IP address
b). root_urlconf is the url config file for the route that points to the project.urls
c). templates, the html templates to clients, all the pages are group together
d). wsgi - django build service
e). databases - db engine with login username, password.
f). auth - server passwords
g). static url - all the assets files

20). urls.py - routing file
21). path(route/ views) the path links to a views or another file for sub-route views as a complete API
22). wsgi - web service gateway interface. how web service communicate with app application and how app application chains process for request

## create first app pages app pull models and html pages together

23). python manage.py startapp pages
24). pages folder is at the same level with main project folder
25). Within the folder
a). migrations - in case there is dbase that migrated, for this app, we won't have any database
b). admin - any info need to show in the admin area. for admin login, we are not applying admin for this app
c). apps.py - PagesConfig function link the app with register under project settings.py file
d). models.py - database structure with all the fields
e). tests.py - for testing
f). views.py - link url to "methods" as "control"

## step 1: Register the app inside the main project folder
