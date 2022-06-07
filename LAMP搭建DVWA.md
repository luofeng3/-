# LAMP搭建DVWA
### LAMP环境搭建
#### apache安装
命令：sudo apt install apache2
启动apache服务：sudo service apache2 start
测试：浏览器输入<IP地址>出现以下页面代表成功
![image-20220607005730836](C:\Users\23033\AppData\Roaming\Typora\typora-user-images\image-20220607005730836.png)
#### mysql安装
命令：sudo apt-get install mysql-server mysql-client
测试：输入 sudo netstat -tap | grep mysql
![image-20220607010229244](C:\Users\23033\AppData\Roaming\Typora\typora-user-images\image-20220607010229244.png)
#### PHP安装
命令:sudo apt install php
测试:php -v
![image-20220607010409706](C:\Users\23033\AppData\Roaming\Typora\typora-user-images\image-20220607010409706.png)

### DVWA安装
#### 1.下载DVWA
命令:git clone  https://github.com/digininja/DVWA (从GitHub克隆到Linux服务器)
![image-20220607010750673](C:\Users\23033\AppData\Roaming\Typora\typora-user-images\image-20220607010750673.png)
#### 2.移动到指定目录( /var/www/html/)
命令:sudo mv DVWA /var/www/html/
注意:普通用户没有权限在/var目录进行操作,命令加sudo或者切换到root用户
#### 3.启动DVWA
浏览器输入:服务器IP地址/DVWA
![image-20220607012541735](C:\Users\23033\AppData\Roaming\Typora\typora-user-images\image-20220607012541735.png)
