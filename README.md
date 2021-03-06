<br>

<p align="center">
<img src="https://git.kancloud.cn/repos/onanying/mixphp1/raw/ba9d4f9d235c24da0a7b8d8a8aa53a57b8e83331/images/logo.png?access-token=1899f10823ef02e1745183298b8c71d3" alt="MixPHP">
</p>

<p align="center">高性能 • 极简 • 多功能</p>

<p align="center">
<img src="https://img.shields.io/badge/downloads-1326-green.svg">
<img src="https://img.shields.io/badge/platform-linux%20%7C%20win%20%7C%20osx-lightgrey.svg">
<img src="https://img.shields.io/packagist/l/doctrine/orm.svg">
</p>

## MixPHP是什么

MixPHP 是秉承 "让每个公司只需使用一种框架" 的理念而创造，采用 Swoole 扩展作为底层引擎，努力打造 Web 开发领域的 "瑞士军刀"。

## 与其他框架的比较

MixPHP 与传统 PHP 的 Web 框架非常不同，MixPHP 可以不需要 Web 服务器(Apache/PHP-FPM)，框架自带 MixHttpd 高性能HTTP服务器，传统的 PHP 应用程序中脚本结束后，所有的对象在请求后都将销毁，而 MixHttpd 不同，框架组件对象常驻于内存，减少对象反复创建销毁的性能损失，具有传统框架无法比拟的性能优势。

MixPHP 也不同于其他基于 Swoole 的全异步服务型框架，只聚焦于 WebService 领域，MixPHP 定位于 Web 开发的全部领域。

MixPHP 更像是传统 Web 框架的次世代版本，拥有更高的性能又保留了快速开发的能力，还能完成传统框架不能想象或者很难实现的功能，比如：多线程、多进程、TCP/UDP服务器。

## 核心特征

* 高性能：极简架构+Swoole引擎，超过Yaf/Phalcon这类C扩展框架的性能，[ [对比测试](http://www.jianshu.com/p/f769b6be1caf) ] ；

* 长连接：按进程保持的长连接，支持Mysql/Redis；

* 服务器：框架自带MixHttpd替代Apache/PHP-FPM作为高性能HTTP服务器；

* 组件：基于组件的框架结构，可通用的Web编程框架；

* 自动加载：完全使用Composer，统一且高效；

* 路由：底层全正则实现，性能高，配置简单；

* 模型：模型集成了使用简单但功能强大的验证器，支持多场景控制；

* 查询构造器：独创的SQL构造方法，可灵活优雅的构造复杂语句；

* 视图：使用PHP做引擎，支持布局、属性；

## 文档

在线手册：[MixPHP开发指南](https://www.kancloud.cn/onanying/mixphp1/379324) | [下载](https://www.kancloud.cn/onanying/mixphp1)

## 环境要求

* PHP >= 5.4
* Swoole >= 1.7.18
* Composer

## 快速开始

一键安装

```
$> php -r "copy('https://raw.githubusercontent.com/mixstart/mixphp/master/installer.php', 'installer.php');include 'installer.php';"
```

输出如下：

```
download mixphp zip ... ok
unzip ... ok
clean temp files ... ok
Successfully installed in "/data/mixphp-master"
```

接下来启动mixhttpd服务器

```
$> cd /data/mixphp-master/server/mixhttpd/
$> php mixhttpd service/start
```

如果一切顺利，运行到最后你将看到如下的输出：

```
                            _____
_______ ___ _____ ___  _____  / /_  ____
__/ __ `__ \/ /\ \/ /  / __ \/ __ \/ __ \
_/ / / / / / / /\ \/  / /_/ / / / / /_/ /
/_/ /_/ /_/_/ /_/\_\ / .___/_/ /_/ .___/
                    /_/         /_/

[2017-09-28 20:59:29] Server    Name: mixhttpd
[2017-09-28 20:59:29] PHP    Version: 5.4.45
[2017-09-28 20:59:29] Swoole Version: 1.9.21
[2017-09-28 20:59:29] Listen    Addr: 127.0.0.1
[2017-09-28 20:59:29] Listen    Port: 9501
```

访问测试：

```
$> curl http://127.0.0.1:9501/
Hello World
```

## 下载

[MixPHP V1 发行版本](https://github.com/mixstart/mixphp/releases)

## 技术交流

官方QQ群：284806582

## License

MixPHP 框架基于 MIT license 进行开源。
