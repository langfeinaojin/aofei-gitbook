---
description: Kettle是绿色软件，客户端只需要解压缩后，无需安装，就可以开始运行。
---

# 客户端工具

Kettle 客户端运行需要 JRE 运行环境，可以运行在windows和Linux平台下。Kettle 包括的几个客户端的功能和启动方式如下：

Windows

* &#x20;     Spoon.bat:  图形界面方式启动作业和转换设计器。

Pan.bat:    命令行方式执行转换。

Kitchen.bat: 命令行方式执行作业。

Carte.bat:   启动web服务，用于 Kettle 的远程运行或集群运行。

Encr.bat:    密码加密

Linux

* &#x20;     spoon.sh  图形界面方式启动

pan.sh:    命令行方式执行转换。

kitchen.sh: 命令行方式执行作业。

carte.sh:   启动web服务，用来远程运行或集群运行。

encr.sh:   密码加密。

说明：

&#x20; 1\. 启动时如果发生 ClassNotFoundException 请使用 java –version检查 jre 的版本是否是1.5 及以上。

&#x20; 2\. 使用远程执行时，要在远程机器上启动 Carte。

&#x20; 3\. 使用集群方式运行时，在集群里的每个机器上都启动 Carte。
