# 在线聊天室

------
@author: 翎羽鹭 (http://www.hellosee.cc)

@email: 1335244575@qq.com

使用swoole扩展和php开发的一个在线聊天室，**目前实现的功能有** ：

> * 支持群聊
> * 支持发送文字
> * 支持发送图片
> * 支持@人
> * 支持分房间聊天功能

在线聊天DEMO：
### [在线聊天室](http://chat.hellosee.cc/)  http://chat.hellosee.cc

# 如何运行？

1.先将client目录放置在您的web服务器下，打开client/static/js/init.js 文件，将该文件的配置修改成自己的域名或者IP

2.打开server目录，首先将rooms目录以及其子目录权限设为777，确保该目录可写。

3.修改server/config.inc.php 文件。将下面两行代码修改为您的域名或者IP。

> define("DOMAIN","http://192.168.56.133:8081");

> define('ONLINE_DIR','/mnt/hgfs/swoole/chatroom/rooms/');

4.命令行执行 ：
> /usr/local/php/bin/php /path/server/hsw_server.php 

# 资料说明
swoole官网 http://www.swoole.com
程序聊天界面采用 钉钉 http://dingtalk.com 

本程序使用的是文件存储。没有测试抗压能力，并且可能存在BUG，切勿用做商业用途。只提供一起学习和讨论。
如果您有问题，欢迎联系QQ：1335244575 共同学习
