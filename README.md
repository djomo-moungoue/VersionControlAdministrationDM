# VersionControlAdministrationDM

# Git

To open the documentation page of a git command online, type the following command:
~~~sh
git CommandName --help
~~~

Push a local branch that is not yet referenced in .git/config file
~~~sh
git push --set-upstream remote BranchName
~~~
The command above will add the following entry in .git/config file
~~~
[branch "BranchName"]
	remote = origin
	merge = refs/heads/BranchName
~~~

Set the correct commiter after mistakenly commiting with the wrong one
~~~sh
# Edit the name and email of the global commiter on the local machine
git config --global --edit

# reset the name and email of the previous commit (not yet pushed) to the current correct global commiter
git commit --amend --reset-author

# The Vim editor command to enter the edit mode is i
# The Vim editor command to save your changes is esc then :wq
# Meaning: escape (esc) the interactive mode (i) the save the changes (w) and quit the vim editor (q).
~~~

Set the name and the email of the global commiter on a local computer
~~~sh
git config --global user.name "user-name"
git config --global user.name@domain
~~~

# GitHub
