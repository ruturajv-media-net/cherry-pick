# GIT Cherry Pick

Apply the changes introduced by some existing commits

```
$ git cherry-pick <commit-id>
$ git cherry-pick -n <commit-id> // To disable auto-commit
```

## Explanation

Explain that every cherry pick is almost a new merge which results in a series of commits. 
To avoid it use -n options so that they can be committed together in a row manually

Show ```~/code/git-cherry-pick```
Show contents of a, b, c, and b2

```
$ git co master
// Try to merge the commit “b2” <eba5c0c>
$ git cherry-pick eba5c0c
// Explain why the err, since, b was missing, unable to auto-merge, however it has done the job and waiting
$ git add b2
$ git cherry-pick --continue
$ git g
```