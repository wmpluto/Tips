# Git
## git rebase
对于分支mywork工作了一段时间后，发现了orgin有新的内容更新，这时去同步origin：使用git merge会产生一个"merge commit"，而使用"git rebase"会把你mywork分支里的每个提交都取消掉，并且把它们临时保存为补丁(patch)，然后再把mywork分支更新到新的origin分支，最后把保存的这些补丁应用到mywork分支上。

需要注意的是，git rebase改写了提交历史，如果你的提交历史没有提交到远程repo时，作为私有部分怎么改都无无所谓，但是一旦提交到了远程后，如果再改写提交历史，那么势必会造成冲突，git push时需要使用-f参数。

同时，在github上提交pull request时，为了让自己的提交更简节，也可以用git rebase -- interactive去调整自己的历史commit。
## fast-forward vs squash vs no-ff


## reference
[Git Community Book 中文版-rebse](http://gitbook.liuhui998.com/4_2.html)
[团队开发里频繁使用 git rebase 来保持树的整洁好吗?](团队开发里频繁使用 git rebase 来保持树的整洁好吗?)
[About Git rebase](https://help.github.com/articles/about-git-rebase/)
