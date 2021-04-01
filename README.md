# ccloud_deploy
ccloud deploy project

##安装步骤
###1 修改配置文件 [`config`](config)

- 如果需要https，设置 `_open_ssl=true`，并配置Ip/域名 `_address=[你的IP]`
- 如果使用域名，你需要手动将证书放在 `[部署目录[clt_deploy]]/nginx/letsencrypt/live/[${_address}]/` 目录下:
(1) 私钥命名 `privkey.pem`
(2) 公钥命名 `fullchain.pem`
  
###2 执行部署脚本 [`bash install.sh [可选安装目录]`](install.sh)

###3 卸载 [`bash uninstall.sh [安装的目录]`](uninstall.sh)

##离线安装

###1 在指定目录放入Docker镜像的离线tar包，也可以放在默认目录[pkg](pkg)。

###2 执行[load.sh](load.sh)脚本: `bash load.sh [放镜像的文件夹]`

###3 执行部署脚本 [`bash install.sh [可选安装目录]`](install.sh)
