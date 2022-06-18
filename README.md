# git



## git文档

[git官方文档](./git_guides)

[note](./note.md)

[git commit-message规范](git-message.md)

## github使用技巧
搜索：[Github搜索语法-信息搜集指南.pdf](Github搜索语法-信息搜集指南.pdf)
快捷键：[更多](https://docs.github.com/cn/get-started/using-github/keyboard-shortcuts)
```hot-key
项目内文件搜索：t
到达指定行：l
改动记录：b
快速定位查看内容模块：ctrl+k
聚焦搜索栏：s或/
转到选项卡：g* （如通知gn，代码gc，问题gi等）
```
网页编辑器：按下。或.键（相当于github.com改为github.dev）即可进入vscode浏览器版；或github.com改为github1s.com
在线运行项目：在项目网址前加上gitpod.io/ 即可在线运行调试项目，构建docker镜像

## Problem_Solution

**git push卡住或需要openssh登陆**

> 原因：使用了http或https的方式clone代码到本地，使用http或https的连接方式
>
> 如：git clone https://github.com/loveleaves/git.git
>
> 而ssh方式：git clone git@github.com:loveleaves/git.git
>
> 解决办法：改为**ssh方式**即可，步骤见下：
>
> 查看当前方式：git remote -v
>
> 移除旧的http的origin：git remote rm origin
>
> 再添加新的ssh方式的origin：git remote add origin git@github.com:loveleaves/git.git
>
> 设置一下上游要跟踪的分支：git push --set-upstream origin master
>
> 或不设置一下上游要跟踪的分支则：git push -u origin main



