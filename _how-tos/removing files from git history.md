---
layout: post
title:  "Removing files from git history"
---

During the process of pubblication of code repos of some of my projects, I encountered the problem of having sensible data stored in certain files the repository, like for example dot env files or yaml configuration files.

Eliminating the file, or erasing the sensible data from the files is not enough, in fact the (once upon a time) private data could be accessed through the commit history of the repository.

The solution in this case is rewriting the whole commit history related to that file.

Fortunately git cli offers a command for that, which is `git rm`, that removes files from the working tree and from the index ([git doc page](https://git-scm.com/docs/git-rm)).

> **NOTE**: before applying these commands perform a backup of your repository!

By exploiting `git filter-branch` and passing to it the `git rm` as parameter, you will apply the commandto every branch:

```sh
git filter-branch --force --index-filter 'git rm --cached --ignore-unmatch <path to the file or directory>' --prune-empty --tag-name-filter cat -- --all
```

*Replace `<path to the file or directory>` with the path to `.env` or `application.properties` that you want to delete*

Once that the operation is completed you can forcely push the new git history to your remote branch.

```sh
git push origin --force --all
```

Remind that if you or other people have a local copy of that repository, you will have to `rebase` the repository on the remote branch.




[Source1](https://gist.github.com/gjerokrsteski/e4a10352448158ba827493eb116cda51?permalink_comment_id=3330898) [Source2](https://stackoverflow.com/questions/43762338/how-to-remove-file-from-git-history/55017549#55017549)