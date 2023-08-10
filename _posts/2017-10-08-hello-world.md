---
title: "Week 1: setting up a static website"

# To set og:image:
# image: ...
---

## Introduction

Notes on Internship days
*I have a MacBook Pro Monterey, version 12.0, Apple M1 Pro chip* 
 
Hi all! On this page I will show you how I started with my internship at De Waag. When starting on my first day, I was introduced to Github: a code hosting platform  or a website and cloud-based service that helps developers store and manage their code, as well as track and control changes to their code. It allows developers, researchers, artists and others to collaborate on projects together, while living in completely different spaces in the world. 
Github can do a lot, but as a start for my internship I used it to launch my own website where I post my progress of my internship. You can see it as documentation or a process document. 

In order to start working with Github you need to have a bunch of other programs or platforms that where completely unknown to me. First of I had to start working with the Terminal on my Macbook - something that always felt like a tech-programming kind of thing on my computer and I had the feeling I would break my laptop if I would start giving that Terminal commands. If you have the same as me, and you have no idea how to work with Terminal, Github or what even the two are, here a little explanation of all of the programs I have come across while launching my website on Github:
- Terminal: The terminal is a command line interface (CLI) for Mac Operating Systems. You use terminal all the time (sort of)- but you just don’t know that. For example: when you want to create a folder in your finder on your Mac, you go to file and then new folder. Exactly the same you can do on Terminal by typing in a code that creates that same folder. Terminal is, you can say, the code that allows you to do certain actions on your laptop. If you tell terminal to download a program, create a folder or show an image, the MacBook will do that. In a way you can say that the MacBook is the machine who speaks an unknown language, you speak English and the terminal is the translator between the two. It can bring your language to the MacBook and back, only the language the terminal speaks is code.
- Git: Git is the software that is installed on your computer (if you have Mac you already have git, if you don’t have Mac you don’t have git - therefore you need to download gitbash - see next dot in line). Git is basically a memory card that remembers code. If you are working on a project, you always want to save your progress of the project. Git basically helps you save this on the computer so you can retrieve your progress at any given time. In order to save your progress you can give git a command in Terminal. So for example: you create a folder in terminal by giving a code to the terminal who translates it for the MacBook. Macbook then creates the folder. After the folder is created you want to save your progress so far so you tell the terminal that git should save your actions. Git then saves the codes you have been using. In case after a day the folder gets deleted or anything else happens, git can retrieve the code you have been using to create the folder, you can copy the code and run the process you have done the day before by pasting it again in the terminal. You with me so far? In case you aren’t; watch this tutorial, it really helped me: https://www.youtube.com/watch?v=mJ-qvsxPHpY. 
- Github: a website and cloud-based service that helps developers store and manage their code, as well as track and control changes to their code. Basically: if you have your written code on your laptop, you can push it or upload it to the cloud of codes: GitHub. Now others can check your code and make changes if needed. They in turn can then push/upoad the updated version of the code online which you can then again check. If you like to new code, you can download it and put it on your laptop. An explanation of Github that really helped me is here: https://www.youtube.com/watch?v=mJ-qvsxPHpY. In order to use GitHub you need to have git installed on your MacBook. 
- Gitbash: Gitbash is the thing you download if you have a non-macbook computer and you need to have Git on your laptop. 
Repository on Github: Repository is basically your online folder. It is the place where you store codes that you have launched on your laptop. It can be for example the folder that holds all the codes in order to create you website. 
- Jekyll: Jekyll is one of many static site generators. I choose to use Jekyll since many of the other interns used it as well and that made it easily accessible. What Jekyll does is it takes text written in your favourite markup language and uses layouts to create a static website. With Jekyll you can basically tweak the site’s look, feel, URL’s, data displayed on the page and much more. In order to use Jekyll, you need to have Ruby installed on your MacBook. 
- Ruby: Ruby is a programming language (code language) you can use. Other programming languages are Python or Java. Macbook already uses Ruby, but a quite old version of it. If you want to check your ruby version on your Mac, you can type "ruby -v” on your terminal. My version was ruby 2.6.3. Since Jekyll is only working with Ruby 2.5 or higher and a little update on Ruby can never do any harm, I decided to update Ruby on my Macbook. 
- RubyGems: RubyGems is basically the library of Ruby. You can see it a bit as the dictionary book ruby has on its side. It enriches the Ruby language. You also need it before using Jekyll.
- Homebrew: Home-brew is a program on your computer that helps you install other programs easily. It basically installs what Apple did not install, but what you do need to start code. 
- Chruby: Chruby is a version manager that helps you install different versions of Ruby and easily switch between them. If you want to update Ruby, also install Chruby
Visual Studio Code: Visual Studio Code is a program that helps your write/modify the website on your computer. 


## Basic codes

Now that you know the basic meanings of the programms we can start with some basic code language that you will need/I have learned during setting up my own GitHub:
- *enter*: After every code you have to type *enter* to command terminal to execute the command
*name of a programm -v*: you see the version of the program that you wish to know the version off
*cd name folder*: means change directory to the folder you wish to go to. You can navigate from folder to folder with this code. Say for example you want to open your documents, you can type cd documents. The Terminal will bring you to your documents then. Now you can make changes in that folder. 
*ls*: With this code you ask Terminal to create a list of all the folders that are in your opened folder. Say for example you want to open your documents and see which folders/files are in your documents, you can type cd documents. The Terminal will bring you to your documents then. Now you can type ls to list all the folders and files that are in your documents folder. 


## Setup steps
Now that you know the basic meanings of the programms and you know the basic code language we can start installing some programs etc. to get your website running. See all my steps below


A. Creating a GitHub account
1.	Create a GitHub account on https://github.com/


B. Create your local and remote GitHub repository
1.	Create a repository on your GitHub account by clicking on the top right corder after being logged in on the + sign and click “new repository”
2.	Give your repository a name (by doing this you create immediately an URL for the repository) and description, keep it public, Add a README file, as gitignore use Jekyll, as a license choose MIT license
3.	For non-mac users: download GitBash, for Mac-users: skip this step.
4.	Download GitHub Desktop. This is an app that communicates between your local repository and your remote repository
5.	Link your remote repository to your local repository by going to the GitHub Desktop
a.	File - Clone repository - type in the name of the repository your created (you did this in step B2) and find the right place to save your local repository (I made a separate folder for this).


C. Downloading Jekyll on your laptop. 
1.	Check if your computer has the prerequisites to run Jekyll. This can be done by checking if your computer has Ruby, RubyGems, GCC and Make. I know these are a bunch of names that might not say much to you know (they didn’t when I first saw them) but no stressy for the dressy: you’ll come around.
2.	To check whether you have Ruby, RubyGems, GCC and Make you open Terminal. While being in terminal you type: ruby -v. By giving the terminal this code: [name of the programm] -v you ask the terminal which version of Ruby your laptop has. Do the same with rubygems -v, GCC -v and MAKE -v. (Type all of them in separately). 
3.	Your MacBook will reply in the terminal that it probably has Ruby version 2.6 or lower and no rubygems, GCC and MAKE. It will say this by giving an error or a false. For using Jekyll on your laptop you need to have a good running Ruby version (it runs on 2.5 or higher). This is why I recommend to update your ruby version (to 3.3) since the one on Mac is quite old and just doesn’t operate properly. In the steps below I will first go into updating Ruby, after which I will dive into Rubygems, GCC and MAKE. 
i.	To install Ruby you first need to install Home-brew. Home-brew is a program on your computer that helps you install other programs easily. It basically installs what Apple did not install, but what you do need to start code with Ruby. To Install Home-brew go to Terminal and paste in the link that can be found on their website: https://brew.sh/. Let Home-brew install (this can take 5 mins or so)
ii.	After installing Home-brew you have to install chruby and ruby install in order to update Ruby. Chruby is a version manager that helps you install different versions of Ruby and easily switch between them. Ruby Install is basically the installation package for Ruby. Both can be done by writing down a code in your terminal: brew install shrubby ruby-install
iii.	After installing Home-brew, Chruby and Ruby Install, you can install Ruby by giving the Terminal a new code: ruby-install ruby 3.1.3
iv.	Now you need to let your shell know that it automatically needs to use Chruby. This you do by first checking if you laptop runs on bash or on zshrc. You can check this by giving the terminal another code: echo $0. Your Terminal will then responds with bash or zsh. After knowing what runs your laptop, you can pasting the following code in your terminal if you laptop runs on zsh. Does your laptop run on bash? Then change the zshrc at the end of the first two sentences to .bash_profile
1.	echo "source $(brew --prefix)/opt/chruby/share/chruby/chruby.sh" >> ~/.zshrc
2.	echo "source $(brew --prefix)/opt/chruby/share/chruby/auto.sh" >> ~/.zshrc
3.	
4.	echo "chruby ruby-3.1.3" >> ~/.zshrc # run 'chruby' to see actual version
v.	Now quit your terminal and open it again. Write the code Ruby -v to check if the version is updated.
4.	After installing Ruby, you can install Jekyll by giving the terminal the code gem install jekyll bundler
5.	Now you can check if RubyGems, GCC and MAKE are also installed by opening terminal and writing rubygems -v, GCC -v and MAKE -v. (Type all of them in separately). With me they were now automatically installed. 


D. Download Visual Studio Code (VSC)
1.	Download VSC: https://code.visualstudio.com/
2.	When having VSC downloaded you need to add some extensions in the program. You can do this by opening the program and going to the left top corner to extensions. Here you type in Ruby and Install the first one to pop up (designed by Peng Lv), Code Runner and Install the first one to pop up (designed by Jun Han)GitHub Pull Requests and Issues and install the first one to pop up (designed by GitHub.com)and Remote Repositories (designed by microsoft - it is often already installed).
3.	Open your remote GitHub repository in VSC. You can do this by opening VSC and pressing SHIFT ENTER P. A menu pops up. This menu is your command palette. If you want to do something in VSC, you always go first to your command palette to find the right command to write your code. The command you need right now is called “open remote repository”. Now you can open the repository that you have on GitHub. 
4.	Open your local GitHub repository in VSC. You can do this by opening VSC and going to file, open folder, show local and finding the local Github repository. 
5.	Now you can see on VSC both your local and your remote GitHub repository. You can also switch between them. 

E. Post your first documentation on GitHub
1.	For you first documentation on GitHub you first have to search for a template/theme that you would like to set up your page in. Searching for templates you can do on https://github.com/topics/jekyll-theme?l=ruby
a.	On this page there is a list of themes. You can check out the theme if the designer of the website has put the URL of the output website online. This always looks the same: [name].github.io
2.	After you have checked some websites and have found the theme that you want, you go to “code” and then “download zip”. Open the zip file and copy all the folders inside the main folder. Paste them inside your local GitHub repository (basically the folder that you have created). Now you have a template that you can alter in your local GitHub repository. 
3.	If correct you have connected VSC to your local GitHub repository. Now you have to check whether you also see the changes you’ve made on your local repository change in VSC, if so it means that the connection between your local repository and VSC is working. Now you only gotta make sure the local GitHub repository is connected to your remote GitHub repository. 
4.	Checking whether the local and remote repositories are connected can be done by going to VSC. There you see the changes you made in the local repository. Here you can add/change text however you like and then commit and push it to the remote repository. On your GitHub desktop you can now Fetch (top of the screen two arrows in the circle) the changes you made in VSC. When you have done that you can push those changes to your remote repository. If correct you can now go to your remote repository and check whether the changes are visible. Not clear? This site helped me with that: https://blog.gitnux.com/guides/how-to-push-code-to-github-from-visual-studio-code/


## Websites that helped me
Websites that helped me along the way were mainly documentations of previous interns. These two below really helped me:
- https://asliaydinaksan.github.io/2022/09/05/setting-up-a-personal-website-for-documentation.html
- https://ellasuza.github.io/documentationella/staticsite.html