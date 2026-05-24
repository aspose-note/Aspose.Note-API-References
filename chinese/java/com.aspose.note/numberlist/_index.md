---
title: "NumberList"
second_title: "Aspose.Note for Java API 参考"
description: "表示编号或项目符号列表。"
type: docs
weight: 64
url: /zh/java/com.aspose.note/numberlist/
---

**Inheritance:**
java.lang.Object
```
public class NumberList
```

表示编号或项目符号列表。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [NumberList(String bulletedSymbol, String font, int fontSize)](#NumberList-java.lang.String-java.lang.String-int-) | 初始化 `NumberList` 类的新实例。 |
| [NumberList(String format, byte numberFormat, String font, int fontSize)](#NumberList-java.lang.String-byte-java.lang.String-int-) | 初始化 `NumberList` 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(NumberList other)](#equals-com.aspose.note.NumberList-) | 确定指定的对象是否等于当前对象。 |
| [equals(Object obj)](#equals-java.lang.Object-) | 确定指定的对象是否等于当前对象。 |
| [getFont()](#getFont--) | 获取或设置字体的名称。 |
| [getFontColor()](#getFontColor--) | 获取或设置字体颜色。 |
| [getFontSize()](#getFontSize--) | 获取或设置字体大小。 |
| [getFormat()](#getFormat--) | 获取或设置行标题的格式。 |
| [getLastModifiedTime()](#getLastModifiedTime--) | 获取或设置最后修改时间。 |
| [getNumberFormat()](#getNumberFormat--) | 获取或设置用于一组自动编号对象的数字格式。 |
| [getNumberedListHeader(int sequenceNumber)](#getNumberedListHeader-int-) | 获取编号列表标题。 |
| [getRestart()](#getRestart--) | 获取或设置覆盖列表项自动编号值的数值。 |
| [hashCode()](#hashCode--) | 作为该类型的哈希函数。 |
| [isBold()](#isBold--) | 获取或设置一个值，指示文本样式是否为粗体。 |
| [isItalic()](#isItalic--) | 获取或设置一个值，指示文本样式是否为斜体。 |
| [setBold(boolean value)](#setBold-boolean-) | 获取或设置一个值，指示文本样式是否为粗体。 |
| [setFont(String value)](#setFont-java.lang.String-) | 获取或设置字体的名称。 |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | 获取或设置字体颜色。 |
| [setFontSize(int value)](#setFontSize-int-) | 获取或设置字体大小。 |
| [setFormat(String value)](#setFormat-java.lang.String-) | 获取或设置行标题的格式。 |
| [setItalic(boolean value)](#setItalic-boolean-) | 获取或设置一个值，指示文本样式是否为斜体。 |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 获取或设置最后修改时间。 |
| [setNumberFormat(Byte value)](#setNumberFormat-java.lang.Byte-) | 获取或设置用于一组自动编号对象的数字格式。 |
| [setRestart(int value)](#setRestart-int-) | 获取或设置覆盖列表项自动编号值的数值。 |
### NumberList(String bulletedSymbol, String font, int fontSize) {#NumberList-java.lang.String-java.lang.String-int-}
```
public NumberList(String bulletedSymbol, String font, int fontSize)
```


初始化 `NumberList` 类的新实例。此实例表示项目符号列表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| bulletedSymbol | java.lang.String | 表示项目符号的符号。 |
| font | java.lang.String | 项目符号的字体。 |
| fontSize | int | 项目符号的字体大小。 |

### NumberList(String format, byte numberFormat, String font, int fontSize) {#NumberList-java.lang.String-byte-java.lang.String-int-}
```
public NumberList(String format, byte numberFormat, String font, int fontSize)
```


初始化 `NumberList` 类的新实例。此实例表示编号列表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| format | java.lang.String | 编号标题的格式。 |
| numberFormat | byte | 标题中数字的格式。 |
| font | java.lang.String | 编号标题的字体。 |
| fontSize | int | 编号标题的字体大小。 |

### equals(NumberList other) {#equals-com.aspose.note.NumberList-}
```
public boolean equals(NumberList other)
```


确定指定的对象是否等于当前对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | [NumberList](../../com.aspose.note/numberlist) | 对象。 |

**Returns:**
boolean - 该 `bool`。
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


确定指定的对象是否等于当前对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 对象 | java.lang.Object | 对象。 |

**Returns:**
boolean - 该 `bool`。
### getFont() {#getFont--}
```
public String getFont()
```


获取或设置字体的名称。

**Returns:**
java.lang.String
### getFontColor() {#getFontColor--}
```
public Color getFontColor()
```


获取或设置字体颜色。

**Returns:**
java.awt.Color
### getFontSize() {#getFontSize--}
```
public int getFontSize()
```


获取或设置字体大小。

**Returns:**
int
### getFormat() {#getFormat--}
```
public String getFormat()
```


获取或设置行标题的格式。对于项目符号列表，表示一个项目符号。

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


获取或设置最后修改时间。

**Returns:**
java.util.Date
### getNumberFormat() {#getNumberFormat--}
```
public Byte getNumberFormat()
```


获取或设置用于一组自动编号对象的数字格式。对于项目符号列表应为 null。

**Returns:**
java.lang.Byte
### getNumberedListHeader(int sequenceNumber) {#getNumberedListHeader-int-}
```
public String getNumberedListHeader(int sequenceNumber)
```


获取编号列表标题。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sequenceNumber | int | 编号列表中的序列号。 |

**Returns:**
java.lang.String - 指定序列号的字符串表示。
### getRestart() {#getRestart--}
```
public int getRestart()
```


获取或设置覆盖列表项自动编号值的数值。

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


作为该类型的哈希函数。

**Returns:**
int - 该 `int`。
### isBold() {#isBold--}
```
public boolean isBold()
```


获取或设置一个值，指示文本样式是否为粗体。

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


获取或设置一个值，指示文本样式是否为斜体。

**Returns:**
boolean
### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


获取或设置一个值，指示文本样式是否为粗体。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFont(String value) {#setFont-java.lang.String-}
```
public void setFont(String value)
```


获取或设置字体的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public void setFontColor(Color value)
```


获取或设置字体颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.awt.Color |  |

### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```


获取或设置字体大小。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setFormat(String value) {#setFormat-java.lang.String-}
```
public void setFormat(String value)
```


获取或设置行标题的格式。对于项目符号列表，表示一个项目符号。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


获取或设置一个值，指示文本样式是否为斜体。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


获取或设置最后修改时间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date |  |

### setNumberFormat(Byte value) {#setNumberFormat-java.lang.Byte-}
```
public void setNumberFormat(Byte value)
```


获取或设置用于一组自动编号对象的数字格式。对于项目符号列表应为 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Byte |  |

### setRestart(int value) {#setRestart-int-}
```
public void setRestart(int value)
```


获取或设置覆盖列表项自动编号值的数值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

