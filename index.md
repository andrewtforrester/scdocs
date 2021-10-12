## SC Tech Stack Documentation

Welcome! Whether [you're new](/matthewletter.md) to web development with Simple Charity or you're a seasoned developer and are just looking to debug something, you'll find everything you need here. 

### Resources for Learning

Simple Charity's website is built on a few key technologies. Some are important to learn before you start working on the site, and others are best learned while working on it: 

##### Preliminaries: 

1. The Command Line (Powershell on Windows and Bash/ZSh on Mac). [This](https://www.learnshell.org) is an excellent tutorial for bash. 
2. Understand [Git](https://git-scm.com/doc)
3. Get to know the file system on your machine. 

##### Before you start, you'll probably want to learn about: 

1. Git. Good documentation can be found [here](https://git-scm.com/doc). 
2. HTML/CSS. There are lots of good resources on the internet for learning these but [this](https://www.udemy.com/course/html-css-code-bootcamp/) course is very comprehensive and doesn’t have much of a learning curve. 
3. Craft Basics. Craft here an excellent [intro tutorial](https://craftcms.com/docs/getting-started-tutorial/) which covers everything you’ll need to know to get started. 
4. Tailwind. Tailwind has very excellent [documentation](https://tailwindcss.com/docs). Start be reading the “getting started” and “core concepts” sections, and then reference the rest as needed. 
5. Basic Vue. Their [docs](https://vuejs.org/v2/guide/) are pretty good. [This](https://www.udemy.com/course/vuejs-2-the-complete-guide/) is also a good course. Don’t learn too much yet, you can pick it up as you start to work on the site pretty easily. 
6. Basic Twig Templating. The [twig docs](https://twig.symfony.com/doc/3.x/) are ok, but they cover _way more_ than you’ll need to know. Part 3 of the craft [intro tutorial](https://craftcms.com/docs/getting-started-tutorial/) will cover everything you need to know. 

##### Once you get going, take a look at: 

1. Craft Commerce
2. Advanced Vue
3. Typeform
4. ActiveCampaign

### Dependencies

1. [VSCode](https://code.visualstudio.com). Or if you _really_ like another code editor, you can use that - but VS Code has some very useful plugins that will make your life _much_ easier: 
    - PostCSS Language Support & HTML CSS Support  
    - Live Server  
    - JSON  
    - Headwind  
    - Twig & Twig Language 
    - Vue  
    - Javascript Code Snippets  
2. Git. It's probably on your machine already but you can run `git --version` on mac to check. If it's not installed already, follow the directions [here](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) to install it. 
3. [Tower](https://www.git-tower.com/mac). SC uses a git methodology called _[Gitflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)_, and tower makes Gitflow very intuitive. They offer [free licenses for students](https://www.git-tower.com/students/mac) at accredited universities. If you're very comfortable with git in the command line, this isn't strictly necessary. 
4. [NPM](https://www.npmjs.com) and [NodeJS](https://nodejs.org/en/)
5. [Docker Desktop](https://www.docker.com/products/docker-desktop)
6. [OpenSSH](https://www.openssh.com)
7. [PHP](https://www.php.net)
8. [Composer](https://getcomposer.org)
9. [Querious](https://www.araelium.com/querious)
10. [Windows Only] Windows-NVM
11. [Windows Only] WSL 2  

### Quick Start Guide

1. Open up your terminal, create the working directory for the Simple Charity site, and navigate into it. 
```
mkdir webprojects
cd webprojects
```
2. Clone the Git repository, navigate into it, and switch to the develop branch. 
```
git clone git@github.com:jonathanmelville/simplecharity.git
cd simplecharity
git switch develop
```
3. Explore the file structure a little bit. Once you're done, navigate to the cms directory with `cd cms`. Open the file "example.env" with `nano example.env` and take a look at it. This file contains all of the variables that specify how the site is to run on your machine. Once you're done, exit the file, and run `mv example.env .env`. This will change the file's name to ".env", which is what docker will expect to see when it looks for environment variables. 
4. Launch Docker Desktop. 
5. In the terminal, run the command `make dev`. This will run a routine that install the necessary dependencies on your computer. In docker desktop, you should see something like [this](/dockerrunning.png) after a little bit. 
6. Once you get a message that says "Ready to handle connections" on your terminal output, your development environment is running. In a browser, go to the address `127.0.0.1:8000` or `localhost:8000` to see the site. 
7. You should see a 503 error message. That's because we haven't installed craft yet. Go to `127.0.0.1:8000/admin` and follow the instructions to install it. IMPORTANT: Don't change the environment variables. 
8. Once craft installs successfully, go back to `127.0.0.1:8000`. You should still see an error. That's because we haven't imported the database into querious yet. Go to `simplecharity.org/admin` and log in with your credentials. Navigate to "utilities" on the sidebar and then to "database backup." Check the "download backup" checkbock and click "Backup." This will download a copy of the database onto your machine. Now, open querious. Log in using the credentials in the `.env` file we made earlier. click the plus button in the bottom right, select "new database", and follow the instruction on screen to import the database we downloaded. 
9. Now your site should be able to talk to the database. Stop docker from the terminal, and relaunch it using `make dev`. On all future launches, run `make dev` to start the development environment. 

### Design Guidelines

Once you start making designs or changing existing ones, you'll want to loo kat Simple Charity's [brand](https://drive.google.com/file/d/1uAQ0PEs7yKxXlCuvM_2pOusghSbvkyzZ/view?usp=sharing) and [messaging] guidelines. Note: you won't be able to open these unless you have a Simlpe Charity email address and are logged inot you google account with it. 

### Common Issues

##### Error 503

##### Database Connection Bugs

##### 

### Contact

[Andrew](mailto:andrewforrester@simplecharity.org) (the one who's been struck by lightning) maintains this site and can (probably) answer questions about the SC tech stack and web dev in general. 

Happy coding! 