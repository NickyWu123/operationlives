# 开始

### iap_list.json ..

* 用于配置实际支付计费点的
* 支付SDK只识别此配置文件

```
 "com.koplagames.kopla02.test.099":
    {
        "des":"GemPack",
        "price":"6.0",
        "guid":"910da6e0-bf15-4454-abc2-dbfc474dd914"
    },
```

**计费点名称**

> com.koplagames.kopla02.test.099

**计费点描述**

> "des":"GemPack"

**实际支付价格**

> "price":"6.0"

**唯一标识符(guid)**

> "guid":"910da6e0-bf15-4454-abc2-dbfc474dd914"



### updateverify.json

* 用于提示玩家更新游戏
* 如果配置文件的版本号大于游戏的版本号，则提示更新

```
{
    "version":"9999999",
    "url":"https://m.3839.com/a/121237.htm",
    "message":"新版本内容已更新，请前往官方授权渠道好游快爆App下载更新！",
    "titile":"选择"
}
```

**最低版本号(手机版本号如果低于此数值则会提示升级)**

> "version":"9999999",

**更新链接**

> "url":"https://m.3839.com/a/121237.htm",

**弹窗话语**

> "message":"新版本内容已更新，请前往官方授权渠道好游快爆App下载更新！",

**弹窗话语2**

>"titile":"选择"



### store.json











