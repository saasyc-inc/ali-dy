# 轻量级阿里大鱼扩展包
## package源安装
> `composer require sentiger/ali-dy -vvv`


## 配置
查看阿里大鱼文档

## 使用
```php
$config    = [
    'accessKeyId'     => 'xxxx',
    'accessKeySecret' => 'xxx',
    'signName'        => 'xxx',
    'templateCode'    => 'xxx',
];
$smsClient = new \Yiche\AliDy\SMSDy($config);

$res = $smsClient->sendSMS('17602191131', [
    'TemplateParam' => [
        // 这个里面是短信模板中的变量，根据实际情况设置变量名称
        'code' => 'xx'
    ]
]);

var_dump($res);
```
