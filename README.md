# docker-compose 集成化配置版本

# 使用流程

+ 安装docker
```bash
# 一键脚本安装
sudo curl -sSL https://get.docker.com | sh
```
+ 安装docker-compose
```bash
#ubuntu
sudo apt-get install docker-compose
#centos7
yum install docker-compose
#其他类型/通用安装方法
sudo wget -O /usr/bin/docker-compose https://pan.xxooxxoo.xyz:8444/f/cbd9947cafe14e369977/?dl=1
sudo chmod +x /usr/bin/docker-compose
sudo /usr/bin/docker-compose -v

```
+ 下载代码到服务器
```bash
git clone https://github.com/scjtqs/dnf-docker-compose dnf-docker-compose
cd dnf-docker-compose/通用模式
vim docker-compose.yml
#修改里面的配置，比如 PublicIp 修改成你的公网ip
#修改完成后 记得保存 :wq
```
+ 启动服务 `docker-compose up -d`
+ 查看日志（可选） `docker-compose logs -f`
+ 未完成部分：集成统一登录器