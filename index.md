## Simple Charity Tech Stack Documentation

Welcome! Whether [you're new](/matthewletter.md) to web development with Simple Charity or you're a seasoned developer and are just looking to debug something, you'll find everything you need here. 

### Resources for Learning

Simple Charity's website is built on a few key technologies. Some are important to learn before you start working on the site, and others are best learned while working on it: 

##### Preliminaries: 

1. The Command Line (Powershell on Windows and Bash/ZSh on Mac)
2. Understand Git
3. Get to know the file system on your maachine

##### Before you start, you'll probably want to learn about: 

1. Git
2. HTML/CSS
3. Craft Basics 
4. Tailwind
5. Basic Vue

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
2. Git, if it's not already installed on your machine. 
3. Tower. SC uses a git methodology called _Git Flow_, and tower makes Git Flow very intuitive. They offer free licenses for students at accredited universities. If you're very confortable with git in the command line, this isn't strictly necessary. 
4. NPM and NodeJS
5. Docker Desktop
6. OpenSSH
7. PHP
8. Composer
9. [Windows Only] Windows-NVM
10. [Windows Only] WSL 2  

### Quick Start Guide

1. Open up your terminal and create a new directory 
`mkdir simplecharity/dev`
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







You can use the [editor on GitHub](https://github.com/andrewtforrester/scdocs/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/andrewtforrester/scdocs/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
