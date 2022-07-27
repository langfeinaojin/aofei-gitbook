---
description: 将给定的十进制数返回为字符串
---

# DecimalToString

参数“fix\_zero”指定所有零十进制值均视为有效（缺省情况下，全部由零组成的十进制数将视为无效）（可选）。这包括压缩十进制表示的符号位都为 0 以及都为内容数字的情况。该特性只在“fix\_zero”为 true 时才视为有效。

· **输入**：decimal (decimal) \[,"fix\_zero"]

· **输出**：result (string)

· **示例**。如果【字段选择】步骤的输入数据流中的 mydec 列包含十进制数 00000004.00，那么以下函数将返回字符串“4”：

`DecimalToString(mydec,"suppress_zero")`

如果 mylink.mydec 列包含十进制数 00000004.00，那么以下函数将返回字符串“0000000000000000000000000004.0000000000”。

`DecimalToString(mydec,"fix_zero")`

如果 mylink.mydec 列包含十进制数 00012344.00。那么以下函数将返回字符串“12344”。

`DecimalToString(mydec,"suppress_zero")`

如果 mylink.mydec 列包含十进制数 00012344.00，那么以下函数将返回字符串“0000000000000000000000012344.0000000000”。

`DecimalToString(mydec,"fix_zero")`

如果 mylink.mydec 列包含十进制数 00012344.120，那么以下函数将返回字符串“0000000000000000000000012344.1200000000”。

`DecimalToString(mydec,"fix_zero")`

如果 mylink.mydec 列包含十进制数 00012344.120，那么以下函数将返回字符串“12344.12”：

`DecimalToString(mydec,"suppress_zero")`

如果 mylink.mydec 列包含十进制数 00012344.120，那么以下函数将返回字符串“0000000000000000000000012344.120000000”。

`DecimalToString(mydec)`

如果 mylink.mydec 列包含十进制数 00012344.000，那么以下函数将返回字符串“0000000000000000000000012344.0000000000”。

`DecimalToString(mydec)`
