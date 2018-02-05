# How to git

## About

Our way of working with Git, and some commands allowing the management of the different branches.

## How to clone the project
`git clone url_to_project destination_folder`

## Create a new branch
Set the source branch as the current one. Most often we will create our branches from the development branch. 

`git checkout development`

And then:

`git branch unfrer/myAwesomeFeature`

Then, switch to the brand new branch running:

`git checkout unfrer/myAwesomeFeature`

## I made changes!
Once changes are ready to be sent to the remote server, you must add the desired files to the next commit you will create.  

`git add .`  

If you add the the "." argument, all your edited files will be add to the next commit. You can also add specific files by specifying their path.

Now, you can create your commit running:

`git commit -m "An awesome description"`

Last step, you will push your commit to the remote git server.

`git push -u origin unfrer/myAwesomeFeature`
