# Part 4 Reverting
Dedicated to situations where you feel like _Oops I messed up_
## Fundamentals
``` git reset --hard <old-commit-id>``` <br/>
```git push -f <remote-name> <branch-name>```<br/>
You might end up having a time if the remote-branch-name and your current-branch-name are not attached. 
<br/>
<br/>
```git commit --amend```
You can simply edit the commit messages without altering the commit messages. But what this command seems to Git would look more like a brand new commit, <br/>
since it's not editing the original commit but more so replacing it with a new commit.
<br/>
<br/>
```git reset --soft```
```git rebasing```
Interested in rewriting history? First make sure you understand the consequences of using the command. This command enables a process of reconnecting the<br/>
snapshots, allowing one commit's patch to go ahead of another commit. Instead of merging, this would seem more like reconnecting. 
<br/>

##Additional
### Links
- [Atlassin git amend](https://www.atlassian.com/git/tutorials/rewriting-history#git-commit--amend)
- [Merging versus Rebasing](https://www.atlassian.com/git/tutorials/merging-vs-rebasing)
<br/>

### Notes
1. When prompted with error: ``` src refspec branch does not match any ``` 
One solution is to use ``` git push origin HEAD --force ``` <br/> 
instead of the original second line.
2. A real-world scenario for using rebasing might be to have a "clean history", when you have multiple people working on the same project, you might want to arrange <br/>
their commits to show features added or parts revised.
