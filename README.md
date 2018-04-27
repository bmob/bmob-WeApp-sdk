Bmob 微信小程序SDK
===================
本项目是Bmob 为小程序客户端开发提供 SDK 支持，里面包含实时数据与数据存储相关操作。


### SDK 获取与安装
Bmob 小程序解决方案客户端 [Demo](https://github.com/magic007/wechatAppDemo "Demo") 已经集成并使用最新版的 SDK，并且已经写了大量常见业务代码。需要快速了解的可以从 [Demo](https://github.com/magic007/wechatAppDemo "Demo") 开始。


### 将sdk引入到微信小程序中
----------
> 方法一：
1. 下载将`utils`目录 复制至项目目录下
2. App.js 初始化SDK
```
const Bmob = require('utils/bmob.js');
Bmob.initialize("你的Application ID", "你的REST API Key");
```

> 方法二：
```
npm install -g bower
bower install bmob-weapp
const Bmob = require('./bower_components/bmob-weapp/utils/bmob.js');
Bmob.initialize("你的Application ID", "你的REST API Key");
```


本小程序Sdk 不需要购买任何相关服务器，即可操作数据库与微信小程序打通，开箱即用。如是之前平台老用户则不需重复申请账号，并且打通之前的Android，IOS，等平台数据，本示例整合了常用的功能，开发请按照以下步骤操作。

### 小程序实战学习视频教程

#### 链接地址：
[小程序视频教程](http://doc.bmob.cn/video/index.html#3 "小程序视频教程")

>Tip: 如果你对数据处理要求比较高，可以引入`underscore.js`库。

### 配置AppId和AppSecret
----------
登录网址后台点击`应用`->`设置`->`应用配置`填写```AppID```,`AppSecret`。
>Tip: 如果你的小程序不需要获取用户`open id`功能，则不需要配置。

>### 开发文档
[Bmob 小程序开发文档](http://doc.bmob.cn/data/wechat_app/index.html "开发文档")

----------

#### <i class="icon-file"></i> 版本 v3.6.1

> **Note:**
>
> - 应微信要求，登陆 auth() 函数，不再保存用户头像
>
> - 增加user.getUserInfo()函数， 更新用户昵称头像信息
>
>   ​

#### <i class="icon-file"></i> 版本 v3.6.0

> **Note:**
>
> - 登陆 auth() 函数，增加then回调，如果出现错误，控制台会提示
> - 兼容小程序游戏，去掉hideNavigationBarLoading 相关函数
> - 增加微信支付退款功能
> - 修复批量删除函数必须用Bmob对象Bug

#### <i class="icon-file"></i> 版本 v3.5.0

> **Note:**
> - 数据SDK整合app.js相关功能
> - 数据启用新域名
> - 增加全新socketSDK
> - 优化登陆流程，登陆更加智能
----------
#### <i class="icon-file"></i> 版本 v3.4.1
> **Note:**
> - 修复个别时候图片上传进度不正确
> - 增加分组、统计等功能
> - 增加BQL 查询功能


#### <i class="icon-file"></i> 版本 v3.4.0
> **Note:**
> - 增加获取手机号解密示例
> - 增加小程序客服回复示例


#### <i class="icon-file"></i> 版本 v3.3.2
> **Note:**
> - 修复视频格式Bug
> - 新特性 文件上传增加进度显示

#### <i class="icon-file"></i> 版本 v3.3.1
> **Note:**
> - 增加试试通讯域名wss.bmobcloud.com
> - 聊天室优化部分流程


#### <i class="icon-file"></i> 版本 v3.0.0
> **Note:**
>
> - 此版本主要变动开发者请求API地址，兼容微信白名单工单
> - index代码增加模板消息推送。

#### <i class="icon-file"></i> 版本 v2.1.0
> **Note:**
>
> - 增加日记详细页面
> - 修复小程序点击事件冒泡问题catchtap
> - 首页增加模糊搜索
> - 修复我发布的没显示bug

#### <i class="icon-file"></i> 版本 v2.0.2
> **Note:**
>
> - 增加我发布的
> - 修复部分bug


#### <i class="icon-file"></i> 版本 v2.0.1
> **Note:**
>
> - 图片上传增加批量上传
> - 页面底部增加版权

#### <i class="icon-file"></i> 版本 v2.0.0
> **Note:**
>
> - 增加新接口，生成二维码应用内推广链接
> - 升级UI2.0
> - 增加反馈功能模版

#### <i class="icon-file"></i> 版本 v1.1.0
> **Note:**
>
> - 增加新登录接口，使用请看app.js
> - 增加新图片删除接口，使用请看接口图片上传

#### <i class="icon-file"></i> 版本 v1.0.0
> **Note:**
>
> - 增加微信支付接口，只需填写key即可微信收款


#### <i class="icon-file"></i> 版本 v0.5.0
> **Note:**

> - 修复返回当前用户延时问题
> - 修复修改用户表缓存没更新问题

----------

#### <i class="icon-file"></i> 版本 v0.4.2
> **Note:**

> - 修复短信验证Bug
> - 添加短信验证Demo

----------

#### <i class="icon-file"></i> 版本 v0.4.1
> **Note:**

> - 修复注册跳转错误
> - 增加获取OpenId示例

----------


#### <i class="icon-file"></i> 版本 v0.4.0
> **Note:**

> - 添加接口示例
> - 添加短信发送示例
> -  添加退出账户操作
> -  增加个人信息展示

----------

#### <i class="icon-file"></i> 版本 v0.3.0
> **Note:**

> - 添加微信小程序关联Bmob后端填写key
> -  小程序获取openid

----------

#### <i class="icon-file"></i> 版本 v0.2.0
> **Note:**

> - 修复部分bug
> - 增加文件上传

----------

#### <i class="icon-file"></i> 版本 v0.1.0
> **Note:**

> - 数据增删改查
> - 登录
> - 注册
>-  短信

----------

> **Tip:** 更多信息请查看[官方文档](http://docs.bmob.cn/data/wechatApp/a_faststart/doc/index.html "官方使用文档")  ，如需帮助可以加入小程序讨论QQ群：**118541934**。
