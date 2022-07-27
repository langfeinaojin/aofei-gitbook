# 数据稽核

在ETL 流程处理结束后，通常要通过统计数据比对的功能，查看源和目标的数据是否一致。以保证ETL 过程的准确性。

管理平台提供了数据稽核功能，来实现自动化的数据比对功能。用户可以实现创建多个比较条件，当ETL 过程结束后，通过“刷新”按钮，自动执行多个比对条件。查看是否有异常数据。

在管理平台左侧有“数据稽核”菜单项，选中该菜单项后，在右侧的面板上出现数据稽核的页面，在数据稽核的页面里，可以完成下面的一些操作：

## 添加数据稽核

点击页面上方工具栏中的“添加”按钮，将出现添加数据稽核的对话框，如下图所示：

![](<../../.gitbook/assets/image (50).png>)

![](<../../.gitbook/assets/image (7).png>)

配置分组、描述、测试数据源、参照数据源、测试SQL、参照SQL、稽核字段。填写完毕后点击“确定”按钮，即可增加所配置的数据稽核 ，页面刷新后新增的数据稽核将出现在列表中。

## 刷新数据稽核

点击页面上方工具栏中的“刷新”按钮，自动执行多个比对条件。查看是否有异常数据。