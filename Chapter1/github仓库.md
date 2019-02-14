# 第4节：github仓库

1. 创建github用户

2. 下载git工具

3. 打开git bash，输入命令链接github

   ```
   (```)
      git config --global user.name "xxxx"
      git config --global user.email "xxxxx@qq.com"
   (```)
   ```

   

4. 设置ssh 

   首先检查是否已生成秘钥，如果返回ls有文件则秘钥生成；
   `cd ~/.ssh`
   没有秘钥

   `ssh-keygen -t rsa -C "xxxxx@qq.com"`
   生成过程 按三次回车。（默认路径，默认没有密码登录）
   找相应的路径用笔记本打开id_rsa.pub,得到ssh key公钥；