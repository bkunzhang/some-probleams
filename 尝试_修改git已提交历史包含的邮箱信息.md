## 总结
- 不建议修改整个版本库的邮箱信息，除非紧急情况，`##3`对历史记录有破坏性。
- 建议使用github的noreply邮箱
`git config user.email "{ID}+{username}@users.noreply.github.com"`

## 1. 查看提交历史的邮箱信息
- 执行命令git log
- 或github相应提交历史页面url加上.patch后缀，回车，就可以看到第2行包含用户名和邮箱信息

## 2. 如果只是最后一次提交包含的邮箱错误，可以[参考](https://stackoverflow.com/questions/43863522/your-push-would-publish-a-private-email-address-error)

Setting your email address for every repository on your computer
`git config --global user.email "{ID}+{username}@users.noreply.github.com"`
or Setting your email address for a single repository
`git config user.email "{ID}+{username}@users.noreply.github.com"`

Reset the author information on your last commit:
`git commit --amend --reset-author`

`git push`

## 3. 修改整个仓库的错误邮箱
- [参考](https://help.github.com/en/articles/changing-author-info)
> 不建议使用，对历史记录有破坏性。我在test仓库执行了多次，导致有很多记录重复。不过尝试一下也好。对于不懂的东西要在test库上尝试，具有好奇心，勤动手没问题。告一段落。


