# 开始

### iap_list.json

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

* 用于配置游戏内商店的显示
* 配置游戏运营活动方案
* 价格需要和iap_list.json保持一致，不然会导致显示价格和实际支付价格不一样
* 计费点id和iap_list.json的计费点id也要保持一致

```
    "com.singmaan.terragenesis.initbundles":
    {
        "des_cn":"初始包",
        "des_en":"initialBundles",
        "content":{
            "pluto":1,
            "energy":50,
            "resources":5000000
        },
        "price_cn":55,
        "price_cn_orignial":0,
        "isdaily":0,
        "multiplerewardfristtime":1,
        "nextBundles":"com.singmaan.terragenesis.conspiracybundles",
        "lastday":"2020-09-10",
        "percentoff":0,
        "valuemultiple":0
    },
```

**礼包的唯一标识符**

>  "com.singmaan.terragenesis.initbundles":

**中文描述**

> "des_cn":"初始包",

**英文描述**

> "des_en":"initialBundles",

**包含的礼包内容 **

> "content":{.....}

**礼包内容的物品之一, 其数量为1**

> "pluto":1,

**礼包内容的物品之一, 其数量为50**

> "energy":50,

**礼包内容的物品之一, 其数量为5000000**

> "resources":5000000,

**中文显示价格，此价格用于实际价格**

> "price_cn":55,

**中文显示原价**

> "price_cn":0,

**是否每日都会领取此奖励(0表示购买一次只会获得一次奖励，大于1表示连续N日获得同样奖励)**

> "isdaily":0,

**是否多倍奖励(1表示只会获得一份奖励，大于1表示会获得多份奖励)**

>  "multiplerewardfristtime":1,

**下一个礼包(这个礼包被购买之后，会立即在原位置显示下一个礼包)**

> "nextBundles":"com.singmaan.terragenesis.conspiracybundles",

**最后购买日(包含配置的日期)**

> "lastday":"2020-09-10",

**折扣力度(只用于显示, 50表示折扣力度为50%)**

> "percentoff":0,

**几倍超值(大于1才显示，一般2倍超值才有显示的意义)**

> "valuemultiple":0