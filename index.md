## SC Tech Stack Documentation

Welcome! Whether [you're new](/matthewletter.md) to web development with Simple Charity or you're a seasoned developer and are just looking to debug something, you'll find everything you need here. 

### Resources for Learning

Simple Charity's website is built on a few key technologies. Some are important to learn before you start working on the site, and others are best learned while working on it: 

##### Preliminaries: 

1. The Command Line (Powershell on Windows and Bash/ZSh on Mac)
2. Understand Git
3. Get to know the file system on your machine

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

1. VSCode. Or if you _really_ like another code editor, you can use that - but VS Code has some very useful plugins that will make your life _much_ easier: 
    - PostCSS Language Support & HTML CSS Support  
    - Live Server  
    - JSON  
    - Headwind  
    - Twig & Twig Language 
    - Vue  
    - Javascript Code Snippets  
2. Git. It's probably on your machine already but you can run `git --version` on mac to check. If it's not installed already, follow the directions [here](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) to install it. 
3. [Tower](https://www.git-tower.com/mac). SC uses a git methodology called _[Gitflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)_, and tower makes Gitflow very intuitive. They offer [free licenses for students](https://www.git-tower.com/students/mac) at accredited universities. If you're very comfortable with git in the command line, this isn't strictly necessary. 
4. NPM and NodeJS
5. Docker Desktop
6. OpenSSH
7. PHP
8. Composer
9. [Windows Only] Windows-NVM
10. [Windows Only] WSL 2  

### Quick Start Guide

1. Open up your terminal and create a new directory. 

```
{mkdir webprojects
cd webprojects
mkdir simplecharity
cd simplecharity
}
```
2. CD into your working directory
`cd simplecharity/dev`
3. Clone the git repository into your simplecharity/dev folder, then check out the correct git branch
`git clone git@github.com:jonathanmelville/simplecharity.git .`
`git checkout develop`
4. Launch Docker Desktop, then ensure that the environment (dev) exists
5. Run `docker-compose up`
6. For future launches, start Docker Desktop, cd into your working directory, then run `docker-compose up`


### Contact

[Andrew](mailto:andrewforrester@simplecharity.org) maintains this site and can (probably) answer questions about the SC tech stack and web dev in general. 

Happy coding! 