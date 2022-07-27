---
description: 比较用于排序的两个字符串
---

# Compare

比较可以采用左对齐形式（缺省值），也可以采用右对齐形式。右对齐比较将指定字符串中的数字子串作为数字进行比较。在每个字符串中，数字字符串必须出现相同的字符位置。例如，对字符串 AB100 和 AB99 的右对齐比较结果表明 AB100 大于 AB99，这是因为 100 大于 99。对字符串 AC99 和 AB100 的左对齐比较结果表明 AC99 大于 AB100，这是因为 C 大于 B。

· **输入**：string1 (string)，string2 (string)，\[justification (L or R)]

· **输出**：result (int8)，string1 小于 string2 时为 -1，两者相同时为 0，string1 大于 string2 时返回 1。

· **示例**。如果【字段选择】步骤的输入数据流中的 mystring1 字段包含字符串“AB99”并且 mystring2 字段包含字符串“AB100”，那么以下函数将返回结果 1。

`Compare(mystring1,mystring2,L)`

如果 mystring1 包含字符串“AB99”并且 mystring2 包含字符串“AB100”，那么以下函数将返回结果 -1。

`Compare(mystring1,mystring2,R)`
