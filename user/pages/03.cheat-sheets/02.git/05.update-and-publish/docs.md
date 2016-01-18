---
title: 'Update & Publish'
published: true
taxonomy:
    category:
        - docs
---

#####List all currently conigured remotes

	$ git remote -v
    
#####Show information about a remote

	$ git remote show <remote>
    
#####Add new remote repository, named <remote>

	$ git remote add <shortname> <url>

#####Download all changes from <remote>, but don‘t integrate into HEAD

	$ git fetch <remote>
    
#####Download changes and directly merge/integrate into HEAD

	$ git pull <remote> <branch>
    
#####Publish local changes on a remote

	$ git push <remote> <branch>
    
#####Delete a branch on the remote

	$ git branch -dr <remote/branch>

#####Publish your tags

	$ git push --tags