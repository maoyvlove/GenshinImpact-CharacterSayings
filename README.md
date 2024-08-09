# 这是一个原神角色语录的API

> 该API持续更新中，欢迎你的使用！GitHub更新可能晚于博客，你可以访问：<https://www.maoyv.com/posts/share/genshin_character_api> 查看最新内容。

<img src="https://count.getloli.com/get/@genshin_character_api" />

## 调用方法

|  标题  | 内容 |
|----------|-----------------------------------|
|  API地址  |  https://api.maoyv.com/zhiluoth/qiandao/genshin/ |
| 调用方法 |  https://api.maoyv.com/zhiluoth/qiandao/genshin/?character=[角色名]&id=[语录ID] |
| 调用示例 |  https://api.maoyv.com/zhiluoth/qiandao/genshin/?character=Nilou&id=0 |

## 参数说明

|  名称  | 内容 |
|----------|-----------------------------------|
|  character  |  角色名，中英文皆可。推荐使用英文名，可见下文角色中英文名称对照表。 |
| id |  语录的id，可留空。当id为0或留空时皆表示随机一条语录。 |

## 返回示例

### 成功

**调用地址**  <https://api.maoyv.com/zhiluoth/qiandao/genshin/?character=Nilou&id=0> 

```json
{
    "result": "succeed",
    "id": 21,
    "situation": "感兴趣的见闻·帕蒂沙兰 ",
    "content": "花神大人跳舞的时候，真正的帕蒂沙兰会在她踏足过的地上盛开。…啊，听起来就非常美好，真想见一见这样的场景。",
    "mp3": "https://uploadstatic.mihoyo.com/ys-obc/2022/10/15/16576950/9f6bbd834901970438c64d6ae4b49a32_6150150067340034755.mp3"
}
```

### 无效的角色名

**调用地址**  <https://api.maoyv.com/zhiluoth/qiandao/genshin/?character=test&id=0> 

```json
{
    "result": "error",
    "msg": "参数「character」应为角色名，「test」 不是一个有效的角色名或当前暂未支持该角色的语录。"
}
```

### 无效的Id

**调用地址**  <https://api.maoyv.com/zhiluoth/qiandao/genshin/?character=Nilou&id=100> 

```json
{
    "result": "error",
    "msg": "参数「id」无效！没有对应「id」为「100」的语录。（这是由于「id」过大导致的）"
}
```

### Id不是数字

**调用地址**  <https://api.maoyv.com/zhiluoth/qiandao/genshin/?character=Nilou&id=test> 

```json
{
    "result": "error",
    "msg": "参数「id」必须为数字！"
}
```

## 角色中英文名称对照表

> 由于咱比较懒，所以目前只支持部分。不过如果有想要的角色可以在博客留言，咱看到一定会马上更新~

|  是否支持  | 中文名 |  英文名 |
|---|--------|-----------|
| ✅ | 妮露 | Nilou |
| ✅ | 宵宫 | Yoimiya |
| ✅ | 雷电将军 | RaidenShogun |
| ✅ | 珊瑚宫心海 | SangonomiyaKokomi |
| ✅ | 可莉 | Klee |
| ✅ | 刻晴 | Keqing |
| ✅ | 甘雨 | Ganyu |
| ✅ | 胡桃 | HuTao |
| ✅ | 申鹤 | Shenhe |
| ✅ | 莫娜 | Mona |
| ✅ | 八重神子 | YaeMiko |
| ✅ | 纳西妲 | Nahida |
| ❌ | 空 | Aether |
| ❌ | 荧 | Lumine |
| ❌ | 派蒙 | Paimon |
| ❌ | 琴 | Jean |
| ❌ | 迪卢克 | Diluc |
| ❌ | 温迪 | Venti |
| ❌ | 阿贝多 | Albedo |
| ❌ | 优菈 | Eula |
| ❌ | 安柏 | Amber |
| ❌ | 凯亚 | Kaeya |
| ❌ | 丽莎 | Lisa |
| ❌ | 芭芭拉 | Barbara |
| ❌ | 雷泽 | Razor |
| ❌ | 菲谢尔 | Fischl 
| ❌ | 班尼特 | Bennett |
| ❌ | 诺艾尔 | Noelle |
| ❌ | 砂糖 | Sucrose |
| ❌ | 迪奥娜 | Diona |
| ❌ | 罗莎莉亚 | Rosaria |
| ❌ | 米卡 | Mika |
| ❌ | 七七 | Qiqi |
| ❌ | 钟离 | Zhongli |
| ❌ | 魈 | Xiao |
| ❌ | 夜兰 | Yelan |
| ❌ | 白术 | Baizhu |
| ❌ | 香菱 | Xiangling |
| ❌ | 北斗 | Beidou |
| ❌ | 行秋 | Xingqiu |
| ❌ | 凝光 | Ningguang |
| ❌ | 重云 | Chongyun |
| ❌ | 辛焱 | Xinyan |
| ❌ | 烟绯 | Yanfei |
| ❌ | 云堇 | YunJin |
| ❌ | 瑶瑶 | Yaoyao |
| ❌ | 枫原万叶 | KaedeharaKazuha |
| ❌ | 神里绫华 | KamizatoAyaka |
| ❌ | 荒泷一斗 | AratakiItto |
| ❌ | 神里绫人 | KamizatoAyato |
| ❌ | 早柚 | Sayu |
| ❌ | 九条裟罗 | KujoSara |
| ❌ | 托马 | Thoma |
| ❌ | 五郎 | Gorou |
| ❌ | 久岐忍 | Kukishinobu |
| ❌ | 鹿野院平藏 | ShikanoinHeizou |
| ❌ | 绮良良 | Kirara |
| ❌ | 提纳里 | Tighnari |
| ❌ | 赛诺 | Cyno |
| ❌ | 流浪者 | Wanderer |
| ❌ | 艾尔海森 | Alhaitham |
| ❌ | 迪希亚 | Dehya |
| ❌ | 柯莱 | Collei |
| ❌ | 多莉 | Dori |
| ❌ | 坎蒂丝 | Candace |
| ❌ | 莱依拉 | Layla |
| ❌ | 珐露珊 | Faruzan |
| ❌ | 卡维 | Kaveh |
| ❌ | 夏洛蒂 | Charlotte |
| ❌ | 达达利亚 | Tartaglia |
| ❌ | 埃洛伊 | Aloy|
