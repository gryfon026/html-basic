Introduction
--------

This is repo of my work with **HTML Tutorial for Beginners** by *The Net Ninja* from YT.

[Link to YT course](https://www.youtube.com/watch?v=Y1BlT4_c_SU)

## **Table of contents**

- [Tagging in git](#tagging-in-git)
- [Sharing tags](#sharing-tags)
- [Deleting tags](#deleting-tags)
- [Checking out Tags](#Checking-out-tags)



## Tagging in git
```
    git log --pretty=oneline
    git tag -a v1.2 9fceb02
    git show v1.2
````
### Sharing Tags

By default, the git push command doesn’t transfer tags to remote servers. You will have to explicitly push tags to a shared server after you have created them. This process is just like sharing remote branches — you can run `git push origin <tagname>`.

`git push origin --tags` -- puts all tags at once

### Deleting Tags

Delete tags on **remote** respository: 

1. **intuitive way** -  `git push origin --delete <tagname>`
2. **second way** - `git push <remote> :refs/tags/<tagname>`

```
    i.e. $ git push origin :refs/tags/v1.4-lw
```
Delete tag on **local** respository:

`$ git tag -d <tagname>`

i.e.

`$ git tag -d v1.4-lw`

### Checking out Tags