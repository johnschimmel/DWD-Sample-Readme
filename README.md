# Dynamic Web Development Class Final Project

Part of your final assignment is to post your code on Github. This will allow anyone interested in learning NodeJS to use your code as an example while getting started.

-----------------------

List of requirements for the Final project submission:

### Create a Github Repository for your existing project. 

You can find out how to create a repo, [http://help.github.com/create-a-repo/](http://help.github.com/create-a-repo/)

When you have created a repo you can add a new Git remote path, allowing you to push your code to Github. We use remote paths now when we push to Heroku

To add the Github remote path, adjust the following command to match your repo's address

    git remote add origin git@github.com:GitHubUsername/YourRepoName.git


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

*   How can a person run your code, what is the command to start the server.

-------

### REMOVE SENSITIVE INFORMATION FROM CODE (RESET YOUR REPO)

If you had any passwords in your code, you should remove them and place them in your .env file. For example in your .env file you have a MONGOLAB_URI variable
    
    MONGOLAB_URI=mongodb://.....
    
You can access this variable in your code with the statement (when using foreman start)

    process.env.MONGOLAB_URI
    
Your .env file should be included in your .gitignore file

### RESET THE REPO

Once you have moved sensitive passwords out of your repo. You can reset your repo by removing the .git directory and reinitalizing the repo. In your code directory in terminal, remove the .git directory

**You only need to do this if you have any passwords in your code (outside your .env file)**

**THIS WILL REMOVE ALL COMMIT HISTORY FROM YOUR REPO**

    rm -rf .git
    
Now you can re-initialize the repo knowing that your passwords will not be in the history. In your code directory in terminal.

    git init
    git add .
    git commit -am "reinit"

Now add in the remote paths to PUSH to Heroku and Github, you must replace with your REPO information

    git remote add heroku git@heroku.com:YOUR-HEROKU-APP.git
    git remote add github git@github.com:GITHUB_USERNAME/GIT-REPO.git
    


    


### When finished - push your code repository to Github

--force command will push

    git push --force github
