# 常见问题

## Mac 5000 端已经使用

运行 `pnpm run serve` 命令，报错：

```basic
Error: listen EADDRINUSE: address already in use :::5000
    at Server.setupListenHandle [as _listen2] (node:net:1330:16)
    at listenInCluster (node:net:1378:12)
    at Server.listen (node:net:1465:7)
    at Polka.listen (/Users/gan/Documents/go/go-studio/go-docs/node_modules/.pnpm/vitepress@0.22.3/node_modules/vitepress/dist/node/serve-777539c0.js:65926:22)
    at Object.serve (/Users/gan/Documents/go/go-studio/go-docs/node_modules/.pnpm/vitepress@0.22.3/node_modules/vitepress/dist/node/serve-777539c0.js:65998:35)
```

查询端口占用信息：

```bash
$ lsof -i tcp:5000
COMMAND   PID USER   FD   TYPE             DEVICE SIZE/OFF NODE NAME
ControlCe 619  gan   41u  IPv4 0xdc1c00b5d145923f      0t0  TCP *:commplex-main (LISTEN)
ControlCe 619  gan   42u  IPv6 0xdc1c00ac394446b7      0t0  TCP *:commplex-main (LISTEN)
```

查询端口被哪个程序使用：

```bash
$ ps aux 619
USER   PID  %CPU %MEM      VSZ    RSS   TT  STAT STARTED      TIME COMMAND
gan    619   0.0  0.1 410190048  90624   ??  S    三04下午   1:30.82 /System/Library/CoreServices/ControlCenter.app/Contents/MacOS/ControlCenter
```

在 [network - ControlCenter.app listens to port 5000/tcp on Monterey OS. Is that normal? Why does it do it? - Ask Different](https://apple.stackexchange.com/questions/431154/controlcenter-app-listens-to-port-5000-tcp-on-monterey-os-is-that-normal-why-d) 上得知端口 5000 现在用于 Airplay。

在“系统偏好设置” > “共享”中取消选中“隔空播放接收器”来关闭它。

![](https://cdn.jsdelivr.net/gh/ganzhixiong/img/blog/202205122354426.png)