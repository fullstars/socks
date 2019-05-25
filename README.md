＃下载安装
下载程序：https://github.com/xiaoqidun/socks
下载说明：下载你需要的平台对应操作系统对应构架的程序文件
本软件不需要网络外的任何权限，可以沙盘和最小权限用户运行
由于没有给傻逼杀毒软件交保护费，如果报毒请自行添加白名单

＃使用示范
wget -O socks5server https://github.com/xiaoqidun/socks/raw/master/socks5server_linux_amd64 && chmod +x socks5server
echo username,password > account.auth
./socks5server -auth account.auth

＃启动服务
./socks5server -host 127.0.0.1 -port 1080 -auth account.auth
-host 指定SOCKS5服务端监听地址
-port 指定SOCKS5服务器监听端口
-auth 指定SOCKS5登录认证的文件

＃用户认证
account.auth为示范用户认证文件，点击这里下载account.auth用户认证文件
用户认证文件为UTF-8纯文本文件，每一行代表一个用户，格式：username,password
编辑用户认证文件不需要重启SOCKS5服务器，修改用户认证文件后一分钟内程序自动热加载
匿名SOCKS5服务器，当用户认证文件不存在或者没有任何用户时支持SOCKS5协议规范的不认证
后台运行

＃linux系统
./socks5server -host 127.0.0.1 -port 1080 -auth account.auth >> socks5server.log 2>&1 &
功能支持

基于用户密码的认证
完整支持TCP协议转发
完整支持UDP协议转发
完整支持IPV4协议转发
完整支持IPV6协议转发
技术支持

腾讯扣群：38181604
腾讯扣扣：88966001
腾讯微信：xiaoqidun
电子邮箱：admin@aite.xyz
技术论坛：https://forum.aite.xyz/
