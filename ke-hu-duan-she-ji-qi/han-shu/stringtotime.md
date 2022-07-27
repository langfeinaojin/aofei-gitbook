---
description: 返回给定字符串的时间表示
---

# StringToTime

· **输入**：string (string)，\[format (string)]

· **输出**：result (time)

· **示例**：如果【字段选择】步骤的输入数据流中的 mystring 字段包含字符串“20:06:58”，那么该函数将返回时间 20:06:58。

`StringToTime(mystring)`

如果 mylink.mystring 列包含字符串“20:6:58”，那么该函数将返回时间 20:06:58。

`StringToTime(mystring,"%(h,s):$(n,s):$(s,s)")`
