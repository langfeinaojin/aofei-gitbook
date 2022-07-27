---
description: 以给定的格式返回给定字符串表示的日期
---

# StringToDate

如果字符串包含缺省格式 yyyy-mm-dd 的日期，那么不必指定格式字符串。

· **输入**：string (string) \[,format (string)]

· **输出**：result (date)

· **示例**：如果【字段选择】步骤的输入数据流中的 mystring 字段包含字符串“1958–08–18”，那么以下函数将返回日期 1958–08–18。

`StringToDate(mystring)`

如果 mylink.mystring 列包含字符串“18:08:1958”，那么以下函数将返回日期 1958–08–18

`StringToDate(mystring,"%dd:%mm:%yyyy")`
