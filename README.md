# Dynamic Web Development Class Final Project

Part of your final assignment is to post your code on Github. This will allow anyone interested in learning NodeJS to use your code as an example while getting started.

-----------------------

List of requirements for the Final project submission:

### Create a Github Repository for your project. 

You can find out how to create a repo, [http://help.github.com/create-a-repo/](http://help.github.com/create-a-repo/)

### Prepare your .env file

Remove all sensitive password and private information from your code and put into your own **.env** file. Search your code for the phrase 'process.env'. Where ever this is used it will contain a reference to your .env file. 

### Create sample env.example file

It would be nice to provide an example .env file for people looking at your code. 

*   Create a copy of your .env file and name it env.example. 
*   Open the new env.example file and replace the actual values with placeholders, for example

    MONGOLAB_URI=YOUR_MONGO_LAB_CONNECTION_HERE

### Create a README file

A Github repository can have a README file. This is the quick-guide, instruction manual for using the repo. You can create a README file with plain text or give some styles with [Markdown Syntax](http://daringfireball.net/projects/markdown/syntax)

Save your README file to your root directory (same level as web.js and package.json)

### Your README should include

*   A link to working example on Heroku.com

*   What your code does when the server is started.

*   What dependencies are required to run the code
    *   Package.json
    *   Any Heroku add-ons like MONGOLAB or CRON

*   List your routes, what URLs are made available when your server is turned on.
    
