![](https://raw.githubusercontent.com/squidproxy/snowleopard/master/docs/logo.jpg)


snowleopard - 可变形流量特征、高效稳定的TCP/IP加速方案
=========================

[![Packagist](https://img.shields.io/badge/Version-V1.3.1.9-blue.svg)](https://github.com/squidproxy/snowleopard/releases)
[![Packagist](https://img.shields.io/badge/Designers%20by-Dave%20feng-brightgreen.svg)] (htps://twitter.com/squidgfw)
[![Packagist](https://img.shields.io/badge/Platform-Windows-brightgreen.svg)] (htps://twitter.com/squidgfw)




Squid Description: 

  Squid is a caching proxy for the Web supporting HTTP, HTTPS, FTP, and more. 
  It reduces bandwidth and improves response times by caching and reusing frequently-requested web pages. Squid has extensive access controls and makes a great server accelerator.
 It runs on most available operating systems,
 including Windows and is licensed under the GNU GPL.
 
obfourscator Description: 

   This is a protocol obfuscation layer for TCP protocols.  Its purpose is to
   keep a third party from telling what protocol is in use based on message
   contents.

   Unlike obfs3, obfs4 attempts to provide authentication and data integrity,
   though it is still designed primarily around providing a layer of
   obfuscation for an existing authenticated protocol like SSH or TLS.

   Like obfs3 and ScrambleSuit, the protocol has 2 phases: in the first phase
   both parties establish keys.  In the second, the parties exchange
   super-enciphered traffic.
   
 
[官方主页](http://www.haidaotai.com) | [Twitter](https://twitter.com/squidgfw) | [谷歌社区](https://plus.google.com/communities/101513261063592651175).

snowleopard X1Client


技术支持环境和网络
------------

* Windows
* IOS
* Android
* OSX

服务端环境
------------

* Debian7+
* Ununtu 14+
 

服务端 X4
Installation
------------
```
wget -N --no-check-certificate  https://git.io/vXTHY  -O ./SLSrv.sh && bash SLSrv.sh 

sh SLSrv.sh

```
服务端 X3
Installation
------------
```
wget -N --no-check-certificate https://git.io/vXIUW -O ./SLSrv.sh && bash SLSrv.sh 

```

###  服务端架构
> 风行者系统
>
> > Shell监视程式
>
>  > > C监视程式
>
> > > > obfs4 + Squid


###  客户端架构
> 监听模块
>
> > 代理模块
>
>  > > 心跳模块(C/S同步技术)
>
> > > > AutoUpdate 模块


###  安全架构
> 许可证验证系统(SHA-2)
>
> > squid验证
>
>  > >  RC4加密
>
> > > > obfsproxy加密

## 1.2.0.4.更新日志

* 加入对ADSl网络环境的支持
* 修正了0.2.1 delphi内存管理dll扩展文件缺失的bug
* 优化了功能
* 提供了使用说明文档
* 新加特性: ProxySetting.dll 模块加入对高度匿名的支持  =>0.2.3
* 新加特性: 主菜单加入高度匿名功能 =>0.2.3
* 新加特性:去除引起杀毒软件误报的释放资源功能的函数,改用直接从雪豹当前目录读取PAC文件,效率更高=>0.2.5
* 新加特性: 加入备用服务器功能=>0.2.7
* 新加特性:加入多个服务器节点的检测功能=>0.2.7
* 新加特性: 加入智能切换排错功能=>0.2.7
* 新加特性: 加入保护功能rc4加密=>0.2.9
* 修正特性 修正切换到主服务器出错无法代理的bug=>0.2.10
* 新加特性: 提供动态升级图标功能=>0.2.10
* 新加特性: 加入独有心跳功能,客户端和服务端会同步更新=>0.2.13
* 新加特性: 提高心跳功能算法,客户端服务器菜单无人值守自主切换=>0.2.14
* 修正: 修正备用服务器全局部分bug =>0.2.15
* 新加特性: 加入最具稳定性的混淆技术Obfsproxy套件=>0.2.16
* 新加特性: 优化了启动速度,1秒之内雪豹完成启动,修正了混淆服务器和其他服务器之间切换的bug,去除了切换服务器显示的多余功能=>0.2.17
* 新加特性: 加入安全的许可证验证机制=>0.2.18
* 新加特性: 加入心跳功能监视模块=>0.2.19
* 新加特性: 优化心跳功能算法和使用UPX等压缩技术=>0.2.19.2
* [10/2/2016]新加特性: 服务器默认使用obfs4混淆技术=>0.2.20.0
* [10/3/2016]新加特性: 优化针对混淆服务器的同步系统功能=>0.2.20.1
* [10/3/2016]新加特性: 混淆服务器使用全新全局模式函数=>0.2.20.1
* [10/3/2016]新加特性: 加入对网络状态的判断=>0.2.20.1
* [10/11/2016]新加特性: 加入混淆服务器节点一个=>1.1
* [10/11/2016]新加特性: 添加客户端启动时对负载服务器的判断,若全部超时,退出主程式=>1.1
* [10/11/2016]新加特性: 添加直连模式=>1.1
* [10/11/2016]修正特性: 修正免费许可证验证后端口占用的bug=>1.2
* [10/11/2016]修正特性: 修正选择直连模式不能智能切换的bug=>1.2
* [10/12/2016]修正特性: XML数据直接从服务端读取,解决部分系统杀毒导致的权限问题=>1.2.0.3
* [10/15/2016]修正特性: 修改高速混淆服务器数据同步=>1.2.0.4
* [10/15/2016]修正特性: 加入主界面UI封面故事同步功能=>1.2.0.4
* [10/15/2016]修正特性: 替换雪豹未来使用图标-蜂鸟=>1.2.0.4
* [10/15/2016]修正特性: 许可证过期监视功能-同步=>1.2.0.4
