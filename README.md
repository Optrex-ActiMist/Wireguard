# Wireguard
Wireguard 一键脚本



# 第一步：下载脚本
```
wget -O wireguard.sh https://raw.githubusercontent.com/Optrex-ActiMist/Wireguard/main/wg.sh
```
# 第二步：确保文件可执行
```
chmod +x wireguard.sh
```
# 第三步： 运行脚本
```
./wireguard.sh
```
# 第四步：配置文件 
脚本会在/root/目录里建好一个client.conf的文件，如果使用的是FinalShell连接的服务器，那么就非常的简单了，直接下载这个文件，然后导入WireGuard就可以了。如果不是使用的Finallshell，需要使用cat打印命令将他打印出来，并复制，新建一个txt文档，保存，重命名后缀名为.conf就可以了：
```
cat /root/client.conf
```
# 第五步：再次运行脚本管理或者卸载 Wireguard
```
sudo bash wireguard.sh
```

# 值得注意的是，每一个客户端文件.conf，只能对应一个用户，不能多客户端使用。需要多人使用，请给每个人分配一个.conf文件。


# 源文件：
```
https://get.vpnsetup.net/wg
```
# 源介绍blog：
```
https://cosmileblog.com/105/
```
