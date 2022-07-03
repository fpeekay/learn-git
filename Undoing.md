命令 git commit --amend

secend  edit

有时候我们提交完了才发现漏掉了几个文件没有添加，或者提交信息写错了。 此时，可以运行带有 --amend 选项的提交命令来重新提交：

这个命令会将暂存区中的文件提交。 如果自上次提交以来你还未做任何修改（例如，在上次提交后马上执行了此命令）， 那么快照会保持不变，而你所修改的只是
提交信息。

如果进行了修改 会覆盖之前提交信息

example:
$ git commit -m 'initial commit'
$ git add forgotten_file
$ git commit --amend
最终你只会有一个提交——第二次提交将代替第一次提交的结果


use "git add <file>..." to update what will be committed

取消暂存的文件
use "git restore --staged <file>..." to unstage
取消工作区的修改
use "git restore <file>..." to discard changes in working directory
checkout 