centos7*64 安装openvpn步骤

1.安装更新并设置正确的时间
yum update
timedatectl
timedatectl --help

2.从软件仓库安装 OpenVPN Access Server
yum -y install https://as-repository.openvpn.net/as-repo-centos7.rpm
yum -y install openvpn-as

3. 记下 Web 界面访问和登录凭据
安装openvpn-as软件包后，记下 Admin UI 和 Client UI 地址以及为您的管理用户openvpn随机生成的密码。

4.在Web界面完成配置和设置用户
使用上一步中的信息，连接到 Admin Web UI 并使用openvpn用户和密码登录。

例如：https:// address /admin/
（将地址替换为您服务器的 IP 或 DNS 主机名）

Access Server Admin Web Interface 提供了一个直观的工具来管理 OpenVPN Access Server 的设置。
但第一次访问时，会收到无法确定网站安全性或隐私性的警告。这是意料之中的。Access Server 带有一个自签名的、不受信任的 SSL 证书，以便 Web 服务能够正常运行。
您可以覆盖此警告消息并继续。我们建议您  为您的访问服务器 设置一个有效的 DNS 主机名并安装一个有效的签名 SSL 证书 来解决此消息。

有疑问请参考：https://openvpn.net/vpn-software-packages/centos/
欢迎探讨梯子搭建
Telegram交流:https://t.me/xiaoshen_i
