# 排序记录

点击“排序记录”，将其拖拽到主设计界面中，在主界面上双击“排序记录”图标，进行参数设定。设置界面如下：

![](<../../../.gitbook/assets/image (27).png>)

注意：

排序目录、临时文件前缀、排序大小是排序时的参数，保留默认设置就可。

排序字段只是针对结果集排序，因此位于过滤组件前还是过滤组件后作用是一样的，以下结果是一致的。但从效率的角度来说，应该是先执行过滤，然后对过滤的结果进行排序。

图1：先排序再过滤

![](<../../../.gitbook/assets/image (64).png>)

图2：先过滤再排序

![](<../../../.gitbook/assets/image (35).png>)