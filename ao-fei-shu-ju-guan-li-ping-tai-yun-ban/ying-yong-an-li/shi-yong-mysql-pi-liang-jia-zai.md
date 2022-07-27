# 如何使用MySQL批量加载

 除了常规的SQL方式加载外。 为了提高加载速度，Kettle 提供了主要数据库的流方式的批量加载，如Oracle 批量加载、MySQL批量加载，PostGreSQL批量加载，GreenPlum批量加载等。Kettle 里的各种批量加载步骤使用的分别是各自数据库的加载命令。 如对 Orale 数据库使用的是 SQLLoader 命令，对 PostGreSQL使用的Copy 命令，对 MySQL数据库使用的Load data 命令等等。这些加载命令实际是一种基于流的数据加载方式，将分割好的数据字段，通过流的方式写入到数据库中。

本文主要介绍下，如何使用傲飞云数据管理平台的 【MySQL 批量加载】步骤将数据批量加载到 MySQL 数据库中。

MySQL 批量加载配置如下：

![](<../../.gitbook/assets/image (11).png>)

![](<../../.gitbook/assets/image (12).png>)

例：创建一个有 表输入、流查询，MySQL 批量加载步骤的转换，运行情况如下图所示：

![](<../../.gitbook/assets/image (77).png>)

注意：

对  TDSQL 的分区表不能使用MySQL的批量加载（会报下面不支持的错误），可以在 TDSQL的非分区表上使用。

![](<../../.gitbook/assets/image (40).png>)
