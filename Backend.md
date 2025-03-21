*Backend notes*

**Chapter 1 - Backend Development**

Frontend - interface to make sending the requests easier.
    --User
    --Client (medium you use to access the website / application)
    --Front-end (the website - the interface)

Backend - process the network requests.
    --URL = IP address written in user friendly form, the DNS translates the URL into the actual address which is the IP address in the network which corresponds to another device connected to the network.
    --Devices at IP address = servers connected to the internet to listen to incoming network requests and then send the response back.
    --Browswer receives the response from the server and displays it on the screen.

**Chapter 2 - Basic backend project**

##Needs##

1. Code editor - write the code

2. Node.js - this is the JS runtime to interpret the instructions

3. Docker - allows you to containerize your application. Our code is usually dependent on a specific operating instruction set. This allows us to containerize our code and run it across a bunch of operating systems. Prevents users from running into issues in different operating systems.

##Getting started##

Start with node.js package library

We have to initialize our project as a node.js project
    --Open the terminal
    --check if you have node and node package manager 'node -v' 'npm -v'
    --initialize node package manager 'npm init -y'

What is Express

It's a package with Node.js for running javascript. It's incredibly common.

To install 'npm install express'

This will generate a bunch of files and create a dependency field with the express package listed. The specs for a project need to specify the packages the code is reliant upon.

You don't really need to touch those files - you don't want to mess with those files.

##Initialize a server using express##

To initialize a server using express
   --create a variable 'const express = require('express')'
   --then define the backend application 'const app = express()'
   --define a PORT 'const PORT = 8383'
   --last step is to say 'app.listen(PORT)'

Basically this says hey mr. app listen to requests coming to this location

##Run the file##

Option 1 - tell 'node server.js' to run it and it'll log it to the terminal

Option 2 - add it to the scripts in the package.json like '"dev": "node server.js"' and then run in the terminal 'npm run dev'

Option 3 - if you're regularly making changes to the files you'll want to install 'npm install nodemon' which is a developer dependency which is something not used in production, only in development so it can regularly update without needing to restart the server. 'npm install --save-dev nodemon' and update the package script to be '"dev": "nodemon server.js"' and when you do 'npm run dev' it'll continually update.

##Kill the execution of the server##

ctrl + C keys

#Endpoints

There are two general endpoints, website endpoints accessible through the URL and API endpoints.

For testing website endpoints we can use the URL, for testing API endpoints we need a client emulator. One is called 'REST Client'.
