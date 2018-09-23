# MaxCompute(ODPS) 常用总结
- 特点
    - 结合自身开发
    - 网友总结

- Time : 2018.09.23
- Author : kngines

---
### GIT base commands of pull & push code from github.

#### 1. exec commands as follows:
- ```
    git config --global user.name "kngines";

    git config --global user.email "self-account@163.com"

    ssh-keygen -t rsa -C "self-account@163.com"

    ```

---

#### 2. New SSH key
- 复制 id_rsa.pub 内容
- SSH and GPG keys --> New SSH key

---

#### 3. base commands
- 初始化仓库
    - ``` git init ```

- 克隆远程仓库代码至本地
    - ``` git clone git@github.com:kngines/MaxComputeTips.git ``` 

- 增加新文件/改动至Git本地仓库
    - ``` git add . ```

- 提交最新更改至本地仓库
    - ``` git commit -m "the change tip message" ```
    
- 更新代码至远程仓库
    - ``` git push -u origin master ```