# V2ray for Doprax

* * *

# 目录

- [项目特点](README.md#项目特点)
- [部署](README.md#部署)
- [鸣谢下列作者的文章和项目](README.md#鸣谢下列作者的文章和项目)
- [免责声明](README.md#免责声明)

* * *

## 项目特点:
* 本项目用于在 Doprax 免费服务上部署 V2ray ，采用的方案为 Nginx + WebSocket + VMess/VLess + TLS。官方宣传不限流量，服务启动后永不停机。
* V2ray 核心文件和配置文件作了“特殊处理”，每个项目都不同，大大降低被封和连坐风险
* vmess 和 vless 的 uuid，路径既可以自定义，又或者使用默认值
* 集成哪吒探针，可以自由选择是否安装
* 部署完成如发现不能上网，请检查域名是否被墙，可使用 Cloudflare CDN 或者 worker 解决。

## 部署:
* 注册 [Doprax.com](https://www.doprax.com/signup/)
* 绑定自己的 github 账户，严重建议小号+私库
* 可用到的变量
  | 变量名 | 是否必须 | 默认值 | 备注 |
  | ------------ | ------ | ------ | ------ |
  | UUID         | 否 | de04add9-5c68-8bab-950c-08cd5320df18 | 可在线生成 https://www.zxgj.cn/g/uuid |
  | VMESS_WSPATH | 否 | /vmess | 以 / 开头 |
  | VLESS_WSPATH | 否 | /vless | 以 / 开头 |
  | NEZHA_SERVER | 否 |        | 哪吒探针服务端的 IP 或域名 |
  | NEZHA_PORT   | 否 |        | 哪吒探针服务端的端口 |
  | NEZHA_KEY    | 否 |        | 哪吒探针客户端专用 Key |

![image](https://user-images.githubusercontent.com/92626977/211194045-dd841af7-717e-4b63-b92f-8aae5d5f1fbc.png)
![image](https://user-images.githubusercontent.com/92626977/211194090-c571f7ae-eb49-467e-8287-a9d143142695.png)
![image](https://user-images.githubusercontent.com/92626977/211194055-a89c32af-f4de-48c6-bc03-eaa05aad104a.png)
![image](https://user-images.githubusercontent.com/92626977/211194066-160e40e0-c057-4d41-9d65-9ee6b6513126.png)
![image](https://user-images.githubusercontent.com/92626977/211194099-3a9ad8f5-1258-479b-a52a-09c81a7f0245.png)
![image](https://user-images.githubusercontent.com/92626977/211194103-9444dd49-9f35-424d-8b95-0e70c7247d86.png)


## 鸣谢下列作者的文章和项目:
ifeng 的 v2ray 项目，在此基础上作修改 https://www.hicairo.com https://github.com/hiifeng

## 免责声明:
* 本程序仅供学习了解, 非盈利目的，请于下载后 24 小时内删除, 不得用作任何商业用途, 文字、数据及图片均有所属版权, 如转载须注明来源。
* 使用本程序必循遵守部署免责声明。使用本程序必循遵守部署服务器所在地、所在国家和用户所在国家的法律法规, 程序作者不对使用者任何不当行为负责。
