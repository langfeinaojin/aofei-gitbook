# 定制化界面

## 登陆页

![](<../../.gitbook/assets/image (6).png>)

修改方法：etl资源库sys\_config表

如上图所示：

大标题对应修改login\_title的值

小标题对应修改login\_title\_small的值

图片logo对应修改login\_logo的值，值upload/login\_logo.png。图片文件放到tomcat/webapp/etl\_platform/upload目录下，文件名称为login\_logo.png

## 浏览器网页的title

![](<../../.gitbook/assets/image (85).png>)

修改方法：etl平台服务器路径tomcat\webapps\etl\_platform\static\config.js文件，version键值

## 菜单名称

![](<../../.gitbook/assets/image (83).png>)

修改方法：etl资源库sys\_menu表
