# How to git

## About

Our way of working with Git, and some commands allowing the management of the different branches.

## How to clone the project?
`git clone url_to_project destination_folder`

## I want a new branch! 
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

## Ups! I can't push!
It is possible that other changes have been made by other developer. You need to get these changes from the server running:

`git pull`

## My branch is ready to be merged!
We prefer to merge our branches from the GitHub client. You must click on `new pull request` from the project view. Then select `base` as the target branch of the merge and `compare` the branch with your changes. Then, just click `create pull request`. You need to confirme the merge, or ask to another developper to merge it.

> **Tips!**  
> To avoid conflicts during mergers, it is important to follow a simple process.  
> For example, I want to merge the `unfrer/myAwesomeFeature` branch with `development`.
> * The first step is the merger of `development` on `unfrer/myAwesomeFeature` to be able to manage the possible conflicts locally, on our > own branch.
> * The second step is the creation of the merge request, this time on `development`.
> * Well done!
