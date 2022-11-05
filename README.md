# Web Application of News Source Verification 

## Introduction
This is a guide for anyone who is interested in implementing the codes as well as running the deployed model both on local and Heroku cloud environments.

## Technologies
- Programming Language - Python version 3.9.7
- Web GUI - HTML, CSS, and Javascript for creating the user interface
- Flask Python framework for API development
- Heroku Cloud Platform for the deployment of the model
## Essentials to Learn
- Web GUI - HTML, CSS, and Javascript
- Heroku Cloud Platform

`Note`: You might need to install all the dependencies used for developing this project if you don’t have them installed already on your local machine. See the `requirements.txt` file for the list of required libraries to install in your development environment in order to execute the code.

## Running and Testing the Python App on your Local Machine
- Clone (or download) the project into your local machine.
- Change your working directory to the folder holding the project from your command line: i.e `News-Source-Verification`
- Run `python app.py` from your command line
- Go to the URL shown in the command prompt. In this case: `http://127.0.0.1:5000/`
- You will be able to use the deployed model on your local machine serving through the localhost.

## Deploying the Machine Learning Model on the Heroku Platform
If you want to implement the deployment process that I took to deploy the model on the Heroku platform, the following steps will guide you:
- If you don’t have one already, create an account in Heroku
- Install git 
- Install Heroku CLI (you can check online on how to do this)
- Login to your Heroku account
- Install gunicorn
- Declare app dependencies (see `requirements.txt` file for the list of dependencies for instance). 
- Create Procfile (see `Procfile` file)
- From the command line, change your working directory to the project folder
- Initialize git inside the project (git init)
- Create a new Heroku app (from your Heroku account: you can name this anything you want so far this name has not been taken before). 
- Add files to the GIT repository and deploy
- Browse deployed URL and see if everything is working fine.

## Useful Commands
- If you haven't already, log in to your Heroku account and follow the prompts to create a new SSH public key with the following command through your command line:
`heroku login`
- Create a new Git repository. Initialize a git repository in a new or existing directory with the following commands:
`cd my-project/` (this should be the name of the directory holding your project)
`git init`
`heroku git:remote -a news-source-verification-app` (change the name to the name you have given to your app)
- Deploy your application: Commit your code to the repository and deploy it to Heroku using Git with the following commands:
`git add .`
`git commit -am "make it better"` (you can choose any alias message you want - alias in the “quote”)
`git push heroku master`











