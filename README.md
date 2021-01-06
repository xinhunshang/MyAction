# 特别声明:

-   本仓库发布的 MyActions 项目中涉及的任何解锁和解密分析脚本，仅用于测试和学习研究，禁止用于商业用途，不能保证其合法性，准确性，完整性和有效性，请根据情况自行判断.

-   本项目内所有资源文件，禁止任何公众号、自媒体进行任何形式的转载、发布。

-   sazs34 对任何脚本问题概不负责，包括但不限于由任何脚本错误导致的任何损失或损害.

-   间接使用脚本的任何用户，包括但不限于建立 VPS 或在某些行为违反国家/地区法律或相关法规的情况下进行传播, sazs34 对于由此引起的任何隐私泄漏或其他后果概不负责.

-   请勿将 MyActions 项目的任何内容用于商业或非法目的，否则后果自负.

-   如果任何单位或个人认为该项目的脚本可能涉嫌侵犯其权利，则应及时通知并提供身份证明，所有权证明，我们将在收到认证文件后删除相关脚本.

-   任何以任何方式查看此项目的人或直接或间接使用该 MyActions 项目的任何脚本的使用者都应仔细阅读此声明。sazs34 保留随时更改或补充此免责声明的权利。一旦使用并复制了任何相关脚本或 MyActions 项目的规则，则视为您已接受此免责声明.

    **您必须在下载后的 24 小时内从计算机或手机中完全删除以上内容.** </br>

    > **_您使用或者复制了本仓库且本人制作的任何脚本，则视为`已接受`此声明，请仔细阅读_**


# 说明:

鉴于 lxk0301 大佬的分支因为 fork 过多用于执行 actions 导致被删，为了防范于未然

> 麻烦各位**不要 fork**`不要fork` _不要 fork_ 不要 fork [不要 fork](backup/reposync.md) ,通过下面的方法重新创建分支，同步代码

[此方式亲测可行，请放心食用，点击查看如何使用 reposync 的方式进行同步代码](backup/reposync.md)

[此方式亲测可行，请放心食用，点击查看如何使用 reposync 的方式进行同步代码](backup/reposync.md)

[此方式亲测可行，请放心食用，点击查看如何使用 reposync 的方式进行同步代码](backup/reposync.md)


## 使用教程

1. [按照这个教程进行 reposync](backup/reposync.md)
2. 再在`Settings`-`Secrets`里面添加`JD_COOKIE`
3. 多条 cookie 用`&`隔开，支持无数条 cookie
4. 前三步之后，点击一下右上角的 star（fork 左边那个），让 workflow 运行一次。

上面四步搞定后就不用管了。

更多Secrets配置[点击查看](backup/secrets.md)


> 具体如何取 cookie 如何配置,可参考 [lxk0301 的获取京东Cookies教程](https://github.com/lxk0301/jd_scripts/blob/master/githubAction.md#%E4%BA%AC%E4%B8%9Ccookie)

#### 下方提供使用到的 **Secrets全集合**

| Name                    |   归属      | 说明                                                         |
| :---------------------: | :----------: | --------- | 
| `PUSH_KEY`              |   微信推送    | cookie失效推送[server酱的微信通知](http://sc.ftqq.com/3.version) |
| `BARK_PUSH`             |   BARK推送    | cookie失效推送BARK这个APP,填写内容是app提供的`设备码`，例如：https://api.day.app/123 ，那么此处的设备码就是`123`，再不懂看 [这个图](icon/bark.jpg) |
| `BARK_SOUND`            |   BARK推送    | bark推送声音设置，例如`choo`,具体值请在`bark`-`推送铃声`-`查看所有铃声` |
| `TG_BOT_TOKEN`          |   telegram推送    | tg推送,填写自己申请[@BotFather](https://t.me/BotFather)的Token,如`10xxx4:AAFcqxxxxgER5uw` , [具体教程](https://github.com/lxk0301/scripts/pull/37#issuecomment-692415594) |
| `TG_USER_ID`            |   telegram推送    | tg推送,填写[@getuseridbot](https://t.me/getuseridbot)中获取到的纯数字ID, [具体教程](https://github.com/lxk0301/scripts/pull/37#issuecomment-692415594) |
| `DD_BOT_TOKEN`          |   钉钉推送    | 钉钉推送[官方文档](https://ding-doc.dingtalk.com/doc#/serverapi2/qf2nxq) ,只需`https://oapi.dingtalk.com/robot/send?access_token=XXX` 等于符号后面的XXX， 注：如果钉钉推送只填写`DD_BOT_TOKEN`，那么安全设置需勾选`自定义关键词`，内容输入输入`账号`即可，其他安全设置不要勾选 |
| `DD_BOT_SECRET`         |   钉钉推送    | 密钥，机器人安全设置页面，加签一栏下面显示的SEC开头的字符串 , 注:填写了`DD_BOT_TOKEN`和`DD_BOT_SECRET`，钉钉机器人安全设置只需勾选`加签`即可，其他选项不要勾选,再不懂看 [这个图](icon/DD_bot.png) |
| `COOKIE_IQIYI` |爱奇艺authcookie|爱奇艺cookie中 P00001的值 详情[文字教程](https://www.bilibili.com/read/cv7437179) [视频教程](https://www.bilibili.com/video/BV1B541157DE) 电脑版有效期三个月
| `BILI_USER` |哔哩哔哩账号|B站账号(由于是账号密码登录,不存在Cookie过期,咱不提供过期提醒.)|
| `BILI_PASS` |哔哩哔哩密码|B站密码|
|`COOKIE_52POJIE`|52破解Cookie|chrome开发者工具获取|
|`COOKIE_91WII`|91WIICookie|chrome开发者工具获取|
|`COOKIE_91WII_FORMHASH`|91WII参数|chrome开发者工具获取|
|`COOKIE_GMSXD`|光明随心订Cookie|圈X[脚本](https://raw.githubusercontent.com/qhq/QuanX/master/Scripts/gmsxd.cookie.js)抓取|

## 鸣谢

[@NobyDa](https://github.com/NobyDa) - 京东每日签到

[@lxk0301](https://github.com/lxk0301) - 京东系列其他签到

[@yangtingxiao](https://github.com/yangtingxiao) - 京东排行榜，天天提额

[@Zero-S1](https://github.com/Zero-S1/xmly_speed) - 喜马拉雅极速版签到
