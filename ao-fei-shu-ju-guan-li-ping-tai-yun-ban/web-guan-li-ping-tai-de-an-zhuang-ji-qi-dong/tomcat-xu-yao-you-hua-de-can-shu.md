# Tomcat需要优化的参数

## windows环境

### 服务启动&#xD;

打开bin\service.bat文件

找到set JvmMx=256，修改为set JvmMx=16384

### 控制台启动&#xD;

修改bin目录下catalina.bat文件

在@echo off下一行追加

set JAVA\_OPTS=-Xms4096m -Xmx16384m

linux环境


修改bin目录下catalina.sh文件

在cygwin=false上一行添加

JAVA\_OPTS="-Xms4096m -Xmx16384m"
