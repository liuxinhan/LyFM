LyFM PHP文件管理器
=================================================

LyFM 是一个基于PHP的个人网站文件管理器，采用完全Ajax操作，实现高效的在线文件管理。


## 使用说明

* 首次使用请配置config.php文件
* 修改默认密码
* 建议将程序放在file目录下，nginx和apache伪静态配置请参考范例，IIS请使用PATH_INFO访问。
* 默认访问形式为 http://127.0.0.1/file/index.php/ 请主动添加后缀
* 如果需要修改程序目录请相应修改伪静态规则
* 如果需要增加对其他文本格式的编辑支持，可手动修改js目录下的`LyApi.js`的第一个TextFileExtenName数组
* 如果访问首页跳转到404页面的，如果支持PATH_INFO请主动添加`/index.php/`来访问，否则节哀。

## 问题说明

* 第一次访问可能会跳转到`/Help#DefaultPassword`页面，表示你需要修改默认密码，通过修改配置文件搞定，可以使用MD5形式的函数将`'94a5f0635f5e7163fc23346870d55b52'` 修改为 `md5('123456')` 的形式
* 默认开启出错输出模式，如果有警告或者其他错误信息会详细输出。如果成功良好的运行，你可以忽略它。并将`define('_Debug_', true);`修改为`define('_Debug_', false);`

## LyFM主页

http://www.loveyu.net/LyFm

## 反馈地址

http://www.loveyu.org/2429.html