# 一个不费脑筋的 PingPlusPlus (pingxx) 前后端实例

# 简介
使用一个 SDK，最重要的是能先跑起来，然后再研究细节，这个实例就可以让你轻松测试前端 HTML5 和后端 PHP 的 PingPlusPlus SDK。

## 版本要求
PHP 版本 5.3 及以上

## 你需要
申请一个 [PingPlusPlus](https://dashboard.pingxx.com/register) 帐号。

## 如何跑起来
### 使用 Composer 安装依赖
执行
```
composer update
```

### 添加 App key 和 App ID

修改文件：`server/pay.php`

```php
//你需要设置的
$apiKey = 'YOUR_API_KEY';
$appId = 'YOUR_APP_ID';
```


1. 登录 [https://dashboard.pingxx.com/](https://dashboard.pingxx.com/) 获取 `Test Key` 或者 `Live Key`;

2. 登录后，选中应用，查看应用信息，获取应用 ID (App Id)。

### 启动 Server

你可以使用`Apache` 或 `Nginx` 等 web server 来启动这个实例。

也可以直接使用 PHP 内置 web server 来启动实例。

```
$ php -S 127.0.0.1:8989
```

### 测试支付

访问：`http://127.0.0.1:8989`

输入金额，点击`银联WAP(upmp)` 进行测试，现在你应该已经跑起来了。

想测试别的支付，请查看代码和[文档](https://pingxx.com/guidance)。

