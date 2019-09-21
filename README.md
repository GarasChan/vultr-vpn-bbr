# vultr-vpn-bbr
## 安装shadowsocks
```
wget –no-check-certificate -O shadowsocks.sh https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocks.sh
```
#### 获取读写权限
`chmod +x shadowsocks.sh`
#### 设置 shadowsocks 密码、端口号和加密方式
`./shadowsocks.sh 2>&1 | tee shadowsocks.log`  
密码、端口号、加密方式设置完成后按下任意键开始安装，过程会持续几分钟
#### 输出 VPN 信息即表示安装成功
## 安装bbr
```
wget --no-check-certificate https://github.com/teddysun/across/raw/master/bbr.sh
```
#### 获取读写权限
`chmod +x bbr.sh`
#### 启动 bbr
`./bbr.sh`  
按下任意键开始安装，过程会持续几分钟。<br>
安装完成后会提示重启服务器，这时输入y重启。<br>
待重新连接服务器后输入`lsmod | grep bbr`，看到以下信息表示安装成功。<br>
Congratulation! 后面你就可以快速访问youtube等网站了。
