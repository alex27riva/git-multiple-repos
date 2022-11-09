# Manage multiple repositories at once
## git_pull_all.sh
Pulls all repositories in a folder.

USAGE:  

`./git_pull_all.sh <folder_with_git_repos>`

Let's say we have all git repositories saved in ~/GitHub directory. Then 
run this script like this:

`./git_pull_all.sh ~/GitHub`

## git_status_all.sh
Shows the status of all repositories in a folder. Useful if you need to 
know, which repositories need to be pushed.

USAGE:  
`./git_status_all.sh <folder_with_git_repos>`

## git_push_repo.sh
Pushes a repository to the server.

USAGE:
`./git_push_repo.sh <repo_folder> <commit_message> [commit_description]`
e.g. (if I'm already in a repository directory)

`./git_push_repo.sh . "testing commit message"`


***********************************************

To be able to use these commands without entering full path to them, 
add full path to the scripts to system variables:

  `vim ~/.bashrc` for BASH or `vim .zshrc` for ZSH.

And add this line to the end

  `export PATH="$PATH:${HOME}/GitHub/git-multiple-repos"`

Save and exit (`:wq`).

Reload config
`source ~/.bashrc` for BASH
or
`source ~/.zshrc` for ZSH
