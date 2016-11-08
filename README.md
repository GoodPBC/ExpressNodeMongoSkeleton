## How to Create an Express.js + Node.js + MongoDB CRUD and REST application skeleton

This serves as an instruction book of sorts to help newer developers to start to define their Node + Express development process. The idea is to provide an application framework that is robust enough to be a great starting point for a project, but not heavy to the point where one feels as if they can still grasp the pieces of the puzzle and build upon what we are giving

This tutorial assumes that you already have the latest version of Node.js installed along with Node's NPM

PART 1 - Install Express.js & the express-generator moudule
	a. - Navigate to your command line(Windows) or your Terminal(OSX)
	   - type the command "npm install -g express" -g will install the latest version of express onto yoursystem.
    
    b. - type the command "npm install -g express-generator"  this command installs  a helpful express utility that scaffolds out the file structure of a common express application.

    c. - create an application. First navigate to the desired directory using your command line. enter "express yourAppName" (replace yourAppName with the name you pick for your application). you will see all the files for your project being made.

    d. Now cd into your application directory and run the "npm install" command to install the initial dependencies for your project.

PART 2 - Setup MongoDB
	a. - if you are on a mac the first step is to update your 
	brew by typing the "brew update" command
	
	b. - install mongo with the "brew install mongodb" command
	
	c. - after mongo has been installed you will start mongo  by enter the "mongod" command. you will see Mongo start up. By default, it will always use port 27017
	
	d. Now we will create a new database. YOU NEED TO OPEN A SECOND TERMINAL WINDOW &  type the "mongo" command to enter the mongo shell.

	e. In the same window, type the "use dbname" command (replace the dbname with whatever you want. it will be the name of your database)..
	the terminal window should read:

			yourterminalname:youruser$ mongo
			MongoDB shell version: 2.6.7
			connecting to: test
			> use yournamedb
			switched to db nodewebappdb
			> db
			nodewebappdb
			> show dbs
			admin               (empty)
			local               0.078GB
			nodews4             0.078GB
			nodewebappdb        0.078GB
			> 