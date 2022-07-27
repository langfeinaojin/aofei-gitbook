---
description: 返回用指定的填充字符数填充的字符串
---

# PadString

· **输入**：string (string) padstring (string) padlength (int32)

· **输出**：result (string)

· **示例**。如果【字段选择】步骤的输入数据流中的 mystring1 字段包含字符串“AB175”，那么以下函数将返回字符串“AB17500000”。

`PadString(mystring1,"0",5)`
