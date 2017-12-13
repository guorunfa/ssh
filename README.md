SSH免密码登录配置

- 用git 输入命令  git config --global user.name "liuchao"
- 输入命令        git config --global user.email "liuchao102@163.com"
- 输入命令        ssh-keygen -t rsa -C "liuchao102@163.com"
- 1 然后回车 回车 再回车
- 2 在文件路径 C:\用户\当前用户名\ 找到 .ssh 文件夹
- 3 文件夹中有两个文件：
  - 私钥：id_rsa
  - 公钥：id_rsa.pub
- 4 在 github -> settings -> SSH and GPG keys页面中，新创建SSH key
- 5 粘贴 公钥 id_rsa.pub 内容到对应文本框中
- 5 在github中新建仓库或者使用现在仓库，拿到git@github.com:用户名/仓库名.git
- 6 此后，再次SSH方式与github“通信”，不用输入密码确认身份
