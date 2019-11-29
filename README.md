本项目需要在两个远程仓库中同时维护

- github地址：https://github.com/tomee-oy/tomee-oy.github.io.git

- coding.net仓库地址：https://e.coding.net/tomee/tomee.coding.me.git

添加方式：
> 将`.git/config`中的`[remote "origin"]`改为以下内容：
```json
  [remote "origin"]
    url = https://github.com/tomee-oy/tomee-oy.github.io.git
    fetch = +refs/heads/*:refs/remotes/origin/*
    url = https://e.coding.net/tomee/tomee.coding.me.git
```