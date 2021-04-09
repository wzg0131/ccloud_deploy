# ccloud_deploy
ccloud deploy project

##Install Step
###1 修改配置文件 [config](config)

- `_address` is your ip or domain, such as `192.168.3.112`,`my.test.com`
- if you configure `_open_ssl` as ture, make sure you have a certificate
###
- 如果需要https，设置 `_open_ssl=true`，并配置Ip/域名 `_address=[你的IP]`
- 如果使用域名，你需要手动将证书放在 `[部署目录[clt_deploy]]/nginx/letsencrypt/live/[${_address}]/` 目录下:
(1) 私钥命名 `privkey.pem`
(2) 公钥命名 `fullchain.pem`


###2 执行部署脚本 [`bash install.sh [可选安装目录]`](install.sh)

###3 卸载 [`bash uninstall.sh [安装的目录]`](uninstall.sh)

