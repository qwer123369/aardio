---
title: "获取 IP 信息"
---

#### 使用说明

使用前需要[下载数据库](https://gitee.com/lionsoul/ip2region/tree/master/data)，保存到非中文目录。

#### 示例代码

```aardio
_URL = "https://suiang.cn/aardio/lib/ip2region.tar.lzma"
_IMPORTURL["ip2region"] = _URL

import console; 
import ip2region;
var region = ip2region("\res\ip2region.db");

var ip = ip2region.getIp();
var info = region.getIpInfo( ip );
 
console.varDump( info )
 
console.log( tostring( info ) )
console.pause(true);
```
