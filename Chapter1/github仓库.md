# 第4节：github仓库

1. 创建github用户

2. 下载git工具

3. 打开git bash，输入命令链接github

   ```
   git config --global user.name "xxxx"
   git config --global user.email "xxxxx@qq.com"
   ```

4. 设置ssh 

   首先检查是否已生成秘钥，如果返回ls有文件则秘钥生成；  
   `cd ~/.ssh`  
   没有秘钥          

   `ssh-keygen -t rsa -C "xxxxx@qq.com"`   
   生成过程 按三次回车。（默认路径，默认没有密码登录）  
   找相应的路径用笔记本打开id_rsa.pub,得到ssh key公钥;

   ![blockchain](https://raw.githubusercontent.com/lengsediao/MarkdownPhotos/master/image/ssh-text.png "ssh-text")

5. 给github账号配置ssh key  

   切换到github，展开个人头像的小三角，点击settings，然后打开SSH keys菜单， 点击Add SSH key新增密钥，填上标题（最好跟本地仓库保持一致）    

   1. 创建本地项目文件夹及文件

   2. 建立本地仓库

      * 进入创建的文件夹

      * 执行  git init 初始化      

         初始化成功后你会发现项目里多了一个隐藏文件夹.git

      * 执行命令

        ```
        git add .  // 将所有文件添加进仓库
        git commit -m "name" // 暂存区 双引号内是提交注释（必填）
        git push origin master // 提交推送远程仓库
        git pull --rebase origin master // 命令进行代码合并
        git status //
        ```

6. github上建立仓库

   复制仓库地址

   ![图片](https://raw.githubusercontent.com/lengsediao/MarkdownPhotos/master/image/ssh-address.png)

7. 执行命令

   `git remote add origin https://github.com/***/myBook.git`



​	end...

