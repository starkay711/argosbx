# K

个人定制版一键代理脚本，基于开源项目 [ArgoSBX](https://github.com/yonggekkk/argosbx)（GPL-3.0）修改。

## 在线命令生成器

👉 https://starkay711.github.io/argosbx/

勾选协议、填好参数，一键生成 SSH 安装命令，复制粘贴到 VPS 里回车即装。

## 快速上手

```bash
bash <(curl -Ls https://raw.githubusercontent.com/starkay711/argosbx/main/argosbx.sh)
```

更推荐用上面的生成器页面拼好参数再装，省心。

## 本版定制内容（相对原版）

- **AnyTLS 支持自定义网址**：通过 `ansni` 参数指定 TLS 的 SNI 域名，不填则默认 `www.bing.com`
  - 示例：`ansni="example.com" anpt="" bash <(curl -Ls https://raw.githubusercontent.com/starkay711/argosbx/main/argosbx.sh)`
- 生成器页面默认勾选 VLESS-reality / TUIC / AnyTLS，Reality 域名预填，订阅默认开启

## 特性（继承原版）

- 基于 Sing-box + Xray 双内核自动分配
- 支持主流 VPS 系统（推荐 Ubuntu），SSH 一键安装
- 所有代理协议均无需域名（Argo 固定隧道、CDN 方案除外）
- 15 种 WARP 出站组合，可更换落地 IP、解锁流媒体
- 单协议分享链接、Clash / Mihomo / Sing-box 聚合订阅都支持

已支持协议：Naiveproxy、Vless-xhttp-tls、AnyTLS、Any-reality、Vless-xhttp-reality-vision-enc、Vless-tcp-reality-vision、Vless-xhttp-vision-enc、Vless-ws-vision-enc、Shadowsocks-2022、Vmess-ws、Socks5、Hysteria2、Tuic、Argo 隧道（Vless-ws-vision-enc / Vmess-ws）

## 客户端推荐

- 安卓：[NekoBox](https://github.com/starifly/NekoBoxForAndroid/releases)（全协议支持）、[v2rayNG](https://github.com/2dust/v2rayNG/releases)、Sing-box 官方版
- Windows：[v2rayN](https://github.com/2dust/v2rayN/releases)（全协议支持)、Sing-box 官方版
- iOS：Shadowrocket、OneXray、Sing-box

注：个别协议仅部分客户端支持。

## 声明

本项目基于 [yonggekkk/argosbx](https://github.com/yonggekkk/argosbx) 二次修改，遵循 GPL-3.0 开源协议。
