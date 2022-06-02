**重要的事说三遍**

- 脚本只提供学习交流，请在法律允许范围内使用！！！！<br>
- 脚本只提供学习交流，请在法律允许范围内使用！！！！<br>
- 脚本只提供学习交流，请在法律允许范围内使用！！！！<br>
   
-openvpn服务一键搭建脚本<br>
-[x]官方稳定版<br>

**介绍**<br>
- 一个Shell脚本，集成openvpn搭建，管理，启动，添加账号等基本操作。基于socks5官方的辅助脚本。<br>
- 脚本只提供学习交流，请在法律允许范围内使用！！！！<br>

**系统支持**<br>

- CentOS 7<br>

**复制以下命令执行**<br>

**第一步**<br>
安装更新并设置正确的时间  <br>
- yum update<br>
- timedatectl<br>
- timedatectl --help<br>

**第二步**<br>
从软件仓库安装 OpenVPN Access Server<br>
<pre><code>yum -y install https://as-repository.openvpn.net/as-repo-centos7.rpm</code></pre>
<pre><code>yum -y install openvpn-as</code></pre>

**第三步**<br>

记下 Web 界面访问和登录凭据<br>
安装openvpn-as软件包后，记下 Admin UI 和 Client UI 地址以及为您的管理用户openvpn随机生成的密码。<br>

**第四步**<br>

- 在Web界面完成配置和设置用户<br>
- 使用上一步中的信息，连接到 Admin Web UI 并使用openvpn用户和密码登录。<br>

例如：https:// address /admin/<br>
（将地址替换为您服务器的 IP 或 DNS 主机名）<br>

Access Server Admin Web Interface 提供了一个直观的工具来管理 OpenVPN Access Server 的设置。<br>
但第一次访问时，会收到无法确定网站安全性或隐私性的警告。这是意料之中的。Access Server 带有一个自签名的、不受信任的 SSL 证书，以便 Web 服务能够正常运行。<br>
您可以覆盖此警告消息并继续。我们建议您  为您的访问服务器 设置一个有效的 DNS 主机名并安装一个有效的签名 SSL 证书 来解决此消息。<br>

**写在最后**<br>

- 有疑问请参考：https://openvpn.net/vpn-software-packages/centos/<br>

- Telegram交流:https://t.me/xiaoshen_i<br>
