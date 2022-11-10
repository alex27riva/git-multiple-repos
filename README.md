# Manage multiple repositories at once
A collection of bash script to manage multiple git repository at once.

This repo was forked from [kyberdrb](https://github.com/kyberdrb/git_manage_all_repositories).

## Installation

Add these these lines to your shell configuration:

Edit your config file with `vim ~/.bashrc` for BASH or `vim ~/.zshrc` for ZSH.

  - `export GITHUB_ROOT="$HOME/GitHub"`
  - `export PATH="$PATH:GITHUB_ROOT/git-multiple-repos"`

Save and exit (`:wq`).

Reload config with:
`source ~/.bashrc` for BASH

or

`source ~/.zshrc` for ZSH

## Usage
### git_pull_all
Pulls all repositories in a folder.

`git_pull_all <folder_with_git_repos>`

Using our variable added earlier:

`git_pull_all $GITHUB_ROOT`

### git_status_all
Shows the status of all repositories in a folder.

Useful if you need to know, which repositories need to be pushed.

`git_status_all $GITHUB_ROOT`

### git_push_repo
Pushes a repository to the server.

`git_push_repo <repo_folder> <commit_message> [commit_description]`

e.g. (if I'm already in a repository directory)

`git_push_repo . "testing commit message"`
