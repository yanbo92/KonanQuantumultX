# KonanQuantumultX
一套适用于[Konancloud](https://konan.ml/auth/register?code=b1hZ)（一个机场）的圈X配置文件，当然，这份配置有强烈的个人风格。本`README.md`主要是记载我改了哪些内容，毕竟Github的圈X配置很多，大部分的东西都可以直接嫖来用，但根据机场要做一些适配性的改动。

## [server_remote]



```
 
 https://kosub.ml/link/XXXXXXXXX?list=shadowrocket#emoji=-1&delreg=[\sV0-9\s]&out=KONAN, tag=konanshadowrocket, update-interval=172800, opt-parser=true, enabled=true  
```

该配置项的功能包括如下：

- 从[Konancloud](https://konan.ml/auth/register?code=b1hZ)下载`Shadowrocket`类型的节点列表（当你想看原文本，需要Base64一下），并通过[KOP-XIAO](https://github.com/KOP-XIAO)大佬的资源解析器转化成一份`QuantumultX`可识别的节点列表
- 参数`out=KONAN`为过滤掉包含`KONAN`的节点，因为只是为了同步信息的，并不是真正的节点
- 参数`emoji=-1`为删除掉节点中的国旗emoji
- 参数`delreg=[\sV0-9\s]`为匹配正则表达式，删除对应的内容，类似`V1 V2`，为了节点地区能被其他正则识别，还是干净一点好
- 注：这条配置你肯定无法直接用，url中的`XXXXXXXXX`需要替换为你自己的链接
