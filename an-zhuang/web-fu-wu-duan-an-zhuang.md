# Web服务端安装

**etl\_platform** 是傲飞数据整合平台的 **Web**服务端，配置方法如下：

* **a**) 在 **Mysql**中创建数据库**etl\_platform**（**MySQL**版本**5.1**或**5.5**）
* **b**) 执行建库脚本**tables\_mysql.sql**

将Tomcat 下的 webapps\etl\_platform\dbTables\tables\_mysql.sql的内容拷贝到查询框中，点击运行

* **c**) 修改平台配置文件

platform\_tianyun\webapps\etl\_platform\WEB-INF\application.properties

修改数据库连接的ip、端口、数据库名称、用户名、密码

platform\_tianyun\webapps\etl\_platform\WEB-INF\jdbc.properties

platform\_tianyun\webapps\etl\_platform\WEB-INF\classes\quartz.properties

* **d**) 平台启动

运行 etl\_platform\bin目录下的startup.bat文件，启动平台

* **e**) 修改资源库连接参数

[http://ip:port/etl\_platform](http://ip/:port/etl\_platform) 进入平台（默认用户名/密码 admin/admin），在资源库管理里， 将Default 资源库的连接参数修改为刚创建的 etl\_platform 数据库的连接参数。

* **f**) 数据服务接口的配置文件。

傲飞数据整合平台可以通过 Rest 和 FTP 两种数据访问接口对外提供数据。要使用这种数据接出的功能，需要在mis.app.properties 配置文件里设置FTP 服务器的连接参数。
