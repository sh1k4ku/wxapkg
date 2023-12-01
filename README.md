# wxapkg

微信小程序解密和解包
都是网上的代码，改了一点点wuWxapkg.js

## 提取

### 安卓平台

存放路径：
`/data/data/com.tencent.mm/MicroMsg/{user哈希值}/appbrand/pkg/`

### Windows 

默认小程序的存放路径为：
`C:\Users\{系统用户名}\Documents\WeChat Files\Applet\{小程序的AppID}\`

windows的为加密过的包，可使用decry.py解密：
`python decry.py --wxid  --file __APP__.wxapkg --output dec.wxapkg`

## 解包

`node wuWxapkg.js dec.wxapkg`