# Spoon设计器

Spoon 是Kettle的图形界面客户端设计器，用来设计Kettle 的作业和转换。\
Kettle 里有转换（Transformation）和 作业（Job）两个概念。转换主要是针对数据的各种处理，一个转换里可以包含多个步骤（Step），每个步骤就是一种数据处理方式，如表输入，文件输入，排序，分组，过滤，选择列，拆分列，增加列等等。Kettle 内置了数十种步骤，另外还可以通过插件的方式由用户自定义自己需要的步骤。

作业是比转换更高一级的处理流程，一个作业里包括多个作业项（Job Entry），一个作业项代表了一项工作，常用的作业项有发送邮件，接收邮件，执行shell 脚本，FTP等等。转换也是作业项之一，即一个作业里可以包括多个转换。一个作业项也可以是其他的一个作业，即作业可以嵌套。作业项也可以通过插件的方式由用户自定义。

转换和作业的设计都是通过 Spoon 来完成的，Spoon 设计好的作业可以保存在文件（转换文件以 .ktr 为扩展名，作业文件以 .kjb 为扩展名）里，也可以保存在数据库（资源库）里。

