# Introduction to Netlify

  
  

### Overview

1. Create a github account
2. Install code editor
3. Forking from a repository
4. Install NPM
5. Connect CLI with Netlify
6. Preview Deploy
7. Make some cool changes :taco:
8. Deploy Changes

  

### Creating a GitHub account

  

Click [here](https://github.com/join?source=header-home) and follow the instructions to create a basic Github account. We will only be using Github to fork from a repository, but Github has many valuable features and is an essential tool of any developer’s tool belt.

  

### Installing VScode

  

For the purpose of this demonstration, I will be using VScode as my code editor, but feel free to use any of the other popular options listed below.

  

[Atom](https://atom.io/)

[Sublime Text](https://www.sublimetext.com/)

  

### Forking from a repository

  

Forking from a repository allows you to create a personal copy of the repository and make your own changes.

For this demonstration we will be working off of a pre-existing code repository so we can focus on setting up a Netlify site.

  

#### Steps

1. navigating to the starting repository [here](https://github.com/jamstack-cincinnati/19-hack-cincinnati)

2. Click ‘Fork’ in the top right corner

3. Click your username when prompted for the destination

4. After you’ve forked the repository to your account, you should be redirected to the repository under your account. From here, click the ' Clone or Download’ dropdown and then click the copy to clipboard Icon to the right of the text input field.

5. With the URL for the remote repository copied to your clipboard, open terminal (If you are on a Mac) or command Prompt (If you are on a PC)

6. Then clone the repository to your local filesystem (make sure to replace [YOUR_USERNAME]):

###

	git clone https://github.com/[YOUR_USERNAME]/19-hack-cincinnati.git

Sweet, you now have the repository on your machine!
  
### Install NPM

Before we get started with Netlify we need to install the command line interface (CLI) for Netlify through NPM. 

Download node.js and NPM for your correct operating system [here](https://nodejs.org/en/) 
  
### Connect CLI to Netlify

1. Install the Netlify CLI on your machine with NPM  with the following command
###
	npm install netlify-cli -g

    If you run into a permission error with this, try typing `sudo chown -R $(whoami) ~/.npm` and run the command again.
2. Once that is done installing, run the following command and you should be redirected to a Netlify in your default browser. If you are not automatically logged in, make sure you are logged in on Github. 
###
	netlify login

This command authorizes the Netlify command line interface (CLI) to connect to Netlify. Now that we have everything set up, let's deploy to Netlify!


### Preview forked repository on Netlify

To deploy your site, simply type `netlify deploy` in your terminal, select `Create & configure a new site` with the arrow keys

1. Run `netlify deploy`
2. Select `Create & configure a new site` 
3. Press Enter until you are prompted with `? deploy path`, which is asking for the path to the directory that you would like to deploy up to Netlify. For us, this would be `./www`

Congratulations! You've successfully deployed your first site with Netlify 🚀 

Now let's see how easy it is to make changes and see the updates live!

### Make changes to files

  Change one of the quotes in `Index.html` to whatever you want. Don't forget to change the author! 
#### Bonus

Change the color of the text to something fun, maybe purple.

### Deploy changes

Now that we've made some changes to our local files, it's time to deploy back up to Netlify so we can see the changes live!

