#Learning git

Using VS code there's a view that lets me put a message in and hit commit. I want to learn how to do it without the helper because I think then I'll really understand.

##First notes

Git <> Github

##What is Git
It is a software that comes on your computer on Mac, Windows you have to download GitBash.

Git is a memory card for code.

If you have a project with a bunch of files - you want just like you have a video game you want to save your progress so if you die you don't lose all your progress.

Every so often you want to hit a command to save your progress.

##Do you need to know Git
Yes, it's one of the most basic things. You need to know Git, command line and then how to code

##To use Git you need a few commands
###Initialize folder or project with git
'git init' - this creates a repository - this is like putting a memory card into your gaming system

###How to save
'git add' - you can save everything or just a specific thing. Maybe you put a file name after 'git add' like 'git add index.html' or you can save everything with 'git add .'

95% of cases you'll just do 'git add .'

Technically this adds all files to the staging area

###Commit the changes to memory
'git commit -m '{describe the save}' the message lets you go back to the version you are saving. Example: 'git commit -m 'create new Git markdown'

###Push the updates to GitHub
'git push -u origin main' allows me to push my committed changes.

###Branches
By default all the code is on a main branch and that's just regular, saving the changes to the master memory.

Someone can go off and trail off, you go off and do something on your friends game but you don't want to save it to their main game so they can do it later and then I save it as a new game. That's branching.

Someone can download my code, make changes, and they do it on a different branch.

'git checkout -b {name of branch}'

There will still be a master branch and I can make changes but it won't impact the main changes getting made.

###See all my logs
'git log' is a log of all saved changes with information about those saves like the time and date.

###Go back to previous progress
You'd copy the commit id and use 'git checkout {id}'

The tricky part is when you create a different branch.

##Github
Github is a website where I can save all my progress on the internet so other people can look through all my code.

###Get code onto GitHub
Create account, create repository

It gives you instructions on how to set it up.