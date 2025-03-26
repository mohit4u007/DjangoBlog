# DjangoBlog

This mini project demos a blog app with some basic features like adding user its profile and various other like pagination,particular user post create delete update post and user profile and pic.
I have included the .env file too but my app passsword is incorrect. Various variables have been used in the django app.
This is a typical django app using gunicorn and ngnix to spin web server all using docker containers.
Database was initially sqlite3 but later used postgresql. You just need to change the settings.py file for DATABASES and it will flip. Only step needed is create usperuser first and then a test user. There after you can use posts.json to create dummy posts for both users (assumption made is super user is id 1 and test user is id 2).
For UI access to DB, although not needed but just for browsing I have added agadmin container. So one can access it at localhost:5050 on a browser. And pgadmin username and password details are in the env file. There after one needs to create a server and connect to postgres DB running in a seperate container. Credentials there in env file.