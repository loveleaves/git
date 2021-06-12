# git



## git文档

[git官方文档](./git_guides)



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



