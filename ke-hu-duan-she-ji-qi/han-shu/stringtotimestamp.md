---
description: 返回给定字符串的时间表示
---

# StringToTimestamp

关于本函数用到的时间格式定义，请参考：

{% embed url="https://www.ibm.com/support/knowledgecenter/en/SSZJPZ_11.3.0/com.ibm.swg.im.iis.ds.parjob.adref.doc/topics/r_deeadvrf_date_format.html" %}

· **输入**：string (string) \[format (string)]

· **输出**：result (time)

· **示例**：如果【字段选择】步骤的输入数据流中的 mystring 字段包含字符串“1958–08–08 20:06:58”，那么该函数将返回时间戳记 1958–08–08 20:06:58。

`StringToTimestamp(mylink.mystring)`

如果 mystring 列包含字符串“8/ 8/1958 20: 6:58”，那么该函数将返回时间戳记 1958–08–08 20:06:58。

`STimestamp(mystring, "%(d,s)/%(m,s)tringTo/%yyyy%(h,s):$(n,s):$(s,s)")`
