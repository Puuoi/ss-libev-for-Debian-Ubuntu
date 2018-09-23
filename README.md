# ss-libev-for-Debian-Ubuntu</br> 
由于秋水逸冰网站国内无法访问，所以为有需要的朋友复制发布到github</br> </br> 
### Debian/Ubuntu下shadowsocks-libev一键安装脚本</br> 
</br> 
原文链接：https://teddysun.com/358.html</br> 
</br> 
</br> 
本脚本适用环境：</br> 
系统支持：Debian/Ubuntu</br> 
内存要求：≥128M</br> 
日期：2018 年 06 月 01 日</br> 
</br> 
</br> 
关于本脚本：</br> 
Debian 或 Ubuntu 下一键安装 libev 版的 Shadowsocks 最新版本。该版本的特点是内存占用小（600k左右），使用 libev 和 C 编写，低 CPU 消耗，甚至可以安装在基于 OpenWRT 的路由器上。</br> 
</br> 
</br> 
默认配置：</br> 
服务器端口：自己设定（如不设定，默认从 9000-19999 之间随机生成）</br> 
密码：自己设定（如不设定，默认为 teddysun.com）</br> 
加密方式：自己设定（如不设定，默认为 aes-256-gcm）</br> 
</br> 
</br> 
客户端下载：</br> 
https://github.com/shadowsocks/shadowsocks-windows/releases</br> 
</br> 
</br> 
使用方法：</br> 
使用root用户登录，运行以下命令：</br> 

```
wget --no-check-certificate -O shadowsocks-libev-debian.sh https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocks-libev-debian.sh
chmod +x shadowsocks-libev-debian.sh
./shadowsocks-libev-debian.sh 2>&1 | tee shadowsocks-libev-debian.log
```

</br> 
安装完成后，脚本提示如下：</br> 

```
Congratulations, Shadowsocks-libev server install completed!
Your Server IP        :your_server_ip
Your Server Port      :your_server_port
Your Password         :your_password
Your Encryption Method:your_encryption_method

Welcome to visit:https://teddysun.com/358.html
Enjoy it!
```

</br> 
卸载方法：</br> 
使用 root 用户登录，运行以下命令：</br> 

```
./shadowsocks-libev-debian.sh uninstall
```

</br> 
本脚本安装完成后，已将 Shadowsocks-libev 加入开机自启动。</br> 
</br> 
</br> 
使用命令：</br> 
启动：/etc/init.d/shadowsocks start</br> 
停止：/etc/init.d/shadowsocks stop</br> 
重启：/etc/init.d/shadowsocks restart</br> 
查看状态：/etc/init.d/shadowsocks status</br> 

### VPS推荐</br> 
<a  href="https://www.vultr.com/promo25b/?ref=7519919" target="_blank">Vultr</a>：15+机房，SSD VPS低至2.5$/月，按小时计费，对新手友好，新用户首充10美元赠送25美元。</br> 
<a href="https://bwh1.net/aff.php?aff=36877&pid=43" target="_blank">BandwagonHost（搬瓦工）</a>：美西CN2线路，部分IP支持观看Netflix，特价款仅需19$/月，使用优惠码BWH26FXH3HIQ享6%优惠</br> 
