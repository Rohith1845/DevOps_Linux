Backend
=======

Backend services is resposible for adding the given  values of databases. Backend serice is return in node.js. Hence we need to install node.js

default node.js version is 16

you need to disable node.js 16, we would like install node.js 20 as per cilent requirement

- dnf module disable nodejs -y
- dnf module enable nodejs:20 -y

-dnf install nodejs -y

Configure the application 
Add the user

-useradd Expense

user expense is a function/ deamon user to run the application. we don't use this user to login

also username is matches to our project

let setup app directory:

-mkdir /app

Download the application code to create app directory

- curl -o curl -o /tmp/backend.zip https://expense-builds.s3.us-east-1.amazonaws.com/expense-backend-v2.zip

cd /app

- unzip /tmp/backend

every application is developed by development team will have some common softwares that they us libraries
