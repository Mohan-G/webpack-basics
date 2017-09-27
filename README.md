# webpack-basics
Prerequisites

You need to have Node.js and npm

Support Node v4 - latest
Support npm v3 - latest
Installation

Download the app from releases page

Go to the app directory and install the packages:



npm install

To build 

npm build

Open the index.html in browser and check the changes.
===================================================================================================================================
To initialize the webpack from beginning follow these sreps:

As a Node-based application, Webpack needs both Node and npm (node package manager) to run.
1) Download and install node from nodejs.org.
2) To install npm, open the command line (for example Terminal on Mac) and run:
	sudo npm install -g
3) Then run:
	npm init
You will walk through the process of creating a package.json file. The default settings are alright, so just keep pressing enter. You can always change this later.
When the package.json is created you will see a little document of data. This is where we tell the project everything it needs to know about itself.

4) To add Webpack to the project, run: 
	npm install webpack -D
	
This gets 3 things to happen:
The name Webpack gets added as a dev dependency inside the package.json file (that’s what the -D in the command is for). This tells the project that Webpack is a tool we will use in the development process, not on the actual website.
A new folder called node_modules gets added to the project.
Webpack (a folder of files) appears inside of node_modules.	

Add the following scripts to package.json:
"scripts": {
  "build": "webpack",
  "start": "webpack --watch"
},
This makes it possible to run the project’s Webpack version through npm by running npm run build and npm run start in the command line.


