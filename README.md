# shadowsocks-http-proxy

🕸说明：shadowsocks http代理

```
部署架构：
Client---->http_proxy/https_proxy---> Host（shadowsocks-http-proxy）----aes-256-cfb---->ShadowsSocks Server（Freedom!!!!!!!）

用法

1.config.json配置文件修改

运行前请修改config.json配置文件中 "server"、"server_port"、"password"、"method" key值为自己SS Server配置信息。

2.编译、运行

root@localhost#git clone https://github.com/chromiumer/shadowsocks-http-proxy.git
root@localhost#cd shadowsocks-http-proxy
root@localhost#go build
root@localhost#./shadowsocks-http-proxy -c config.json -proxy_type http

3.客户端命令行代理配置

root@localhost#export http_proxy=http://xx.xx.xx.xx:1080;export https_proxy=http://xx.xx.xx.xx:1080;

4.取消代理配置

root@localhost#unset http_proxy https_proxy

```
