务实一点，先把git的这个理念先搞懂

版本控制器，就是可以控制一堆文件的版本，修改了哪里之类的



工作区：

就是指当前git的目录下的所以文件

暂存区：

就是指add . 之后的区域，add了但没提交这个状态，commit完暂存区就没文件了



HEAD：

当前分支的指针



分支：

就是互不影响的工作区，git很常用的功能。每个分支都有一个指针指向最后提交，切换分支意味着HEAD指向那个分支的指针，例如HEAD->dev

新建分支：

当我们创建新的分支，例如dev时，Git新建了一个指针叫dev，指向master相同的提交，再把HEAD指向dev，就表示当前分支在dev上



合并分支：

快进合并模式：Fast-forward 也就是直接把master指向dev的当前提交。例如主分支没变，其他分支修改后被合并





```
git log --graph --pretty=oneline --abbrev-commit # 查看分支合并情况
git stash # 保持当前工作现场，但不提交
git cherry-pick # 复制特定提交到分支
```



#### 连接

https://www.liaoxuefeng.com/wiki/896043488029600

https://blog.csdn.net/w605283073/article/details/80099644