# xray for Deepnote

![image](https://user-images.githubusercontent.com/122191366/217796228-90fda930-7aa1-4373-8fbd-8b50ec878715.png)

> 总结：要部署的就封号，不部署的就没事

## 项目特点

* 本项目用于在 [Deepnote](https://deepnote.com/) 免费服务上部署 vmess / vless / trojan / shadowsocks 节点
* 部署完成如发现不能上网，请检查域名是否被墙，可使用 Cloudflare CDN 或者 worker 解决。

## 部署

* 注册 [Deepnote](https://deepnote.com/)
* 创建一个Project，点击Environment中的Initialization，打开里面的`init.ipynb`
* 删除里面自带的代码块并创建一个，输入下面的内容

```
!sleep infinity
```

![](https://gcore.jsdelivr.net/gh/Misaka-blog/imgs@main/20230208164251.png)

* 打开 Allow Incoming Connections的开关
* 在命令行复制粘贴，运行以下命令

```shell
wget -N https://raw.githubusercontent.com/Misaka-blog/xray-for-deepnote/main/deep.sh && bash deep.sh
```

* 节点配置如下

```
协议：Vmess / Vless / Trojan / Shadowsocks
地址：xxxxx.deepnoteproject.com
端口：443
UUID/密码：8d4a8f5e-c2f7-4c1b-b8c0-f8f5a9b6c384 或自己定义的UUID
额外ID：0
Shadowsocks加密方式：chacha20-ietf-poly1305
传输协议：ws
伪装域名：xxxxx.deepnoteproject.com
路径：/vmess（/vless、/trojan、/shadowsocks）
传输安全：TLS
跳过证书验证：true或false都可以
```

## 免责声明

* 本程序仅供学习了解, 非盈利目的，请于下载后 24 小时内删除, 不得用作任何商业用途, 文字、数据及图片均有所属版权, 如转载须注明来源。
* 使用本程序必循遵守部署免责声明。使用本程序必循遵守部署服务器所在地、所在国家和用户所在国家的法律法规, 程序作者不对使用者任何不当行为负责。

## 赞助

爱发电：https://afdian.net/a/Misaka-blog

![afdian-MisakaNo の 小破站](https://user-images.githubusercontent.com/122191366/211533469-351009fb-9ae8-4601-992a-abbf54665b68.jpg)
