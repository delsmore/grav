---
title: 'Branches & Tags'
published: true
taxonomy:
    category:
        - docs
---

#####List all existing branches

	$ git branch -av

#####Switch HEAD branch

	$ git checkout <branch>
    
#####Create a new branch based on your current HEAD

	$ git branch <new-branch>
    
#####Create a new tracking branch based on a remote branch

	$ git checkout --track <remote/branch>
    
#####Delete a local branch

	$ git branch -d <branch>
    
#####Mark the current commit with a tag

	$ git tag <tag-name>