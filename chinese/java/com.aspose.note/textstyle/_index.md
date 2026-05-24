---
title: "TextStyle"
second_title: "Aspose.Note for Java API 参考"
description: "指定文本样式。"
type: docs
weight: 93
url: /zh/java/com.aspose.note/textstyle/
---

**Inheritance:**
java.lang.Object, com.aspose.note.Style
```
public final class TextStyle extends Style<TextStyle>
```

指定文本样式。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [TextStyle()](#TextStyle--) | 初始化一个新的 `TextStyle` 类的实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(TextStyle other)](#equals-com.aspose.note.TextStyle-) | 确定指定的对象是否等于当前对象。 |
| [equals(Object obj)](#equals-java.lang.Object-) | 确定指定的对象是否等于当前对象。 |
| [getDefault()](#getDefault--) | 获取具有 "en-US" 区域设置的样式。 |
| [getDefaultMsOneNoteTitleDateStyle()](#getDefaultMsOneNoteTitleDateStyle--) | 获取 MS OneNote 中标题日期的默认样式。 |
| [getDefaultMsOneNoteTitleTextStyle()](#getDefaultMsOneNoteTitleTextStyle--) | 获取 MS OneNote 中标题文本的默认样式。 |
| [getDefaultMsOneNoteTitleTimeStyle()](#getDefaultMsOneNoteTitleTimeStyle--) | 获取 MS OneNote 中标题时间的默认样式。 |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | 获取超链接地址。 |
| [getLanguage()](#getLanguage--) | 获取文本的语言。 |
| [hashCode()](#hashCode--) | 作为该类型的哈希函数。 |
| [isHidden()](#isHidden--) | 获取指示文本样式是否隐藏的值。 |
| [isHyperlink()](#isHyperlink--) | 获取指示文本样式是否为超链接的值。 |
| [isMathFormatting()](#isMathFormatting--) | 获取或设置指示文本样式是否为数学格式的值。 |
| [setHidden(boolean value)](#setHidden-boolean-) | 设置指示文本样式是否隐藏的值。 |
| [setHyperlink(boolean value)](#setHyperlink-boolean-) | 设置指示文本样式是否为超链接的值。 |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | 设置超链接地址。 |
| [setLanguage(Locale value)](#setLanguage-java.util.Locale-) | 设置文本的语言。 |
| [setMathFormatting(boolean value)](#setMathFormatting-boolean-) | 设置一个值，指示文本样式是否为数学格式。 |
### TextStyle() {#TextStyle--}
```
public TextStyle()
```


初始化一个新的 `TextStyle` 类的实例。

### equals(TextStyle other) {#equals-com.aspose.note.TextStyle-}
```
public boolean equals(TextStyle other)
```


确定指定的对象是否等于当前对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | [TextStyle](../../com.aspose.note/textstyle) | 对象。 |

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
### getDefault() {#getDefault--}
```
public static TextStyle getDefault()
```


获取具有 "en-US" 区域设置的样式。

**Returns:**
[TextStyle](../../com.aspose.note/textstyle)
### getDefaultMsOneNoteTitleDateStyle() {#getDefaultMsOneNoteTitleDateStyle--}
```
public static TextStyle getDefaultMsOneNoteTitleDateStyle()
```


获取 MS OneNote 中标题日期的默认样式。

**Returns:**
[TextStyle](../../com.aspose.note/textstyle)
### getDefaultMsOneNoteTitleTextStyle() {#getDefaultMsOneNoteTitleTextStyle--}
```
public static TextStyle getDefaultMsOneNoteTitleTextStyle()
```


获取 MS OneNote 中标题文本的默认样式。

**Returns:**
[TextStyle](../../com.aspose.note/textstyle)
### getDefaultMsOneNoteTitleTimeStyle() {#getDefaultMsOneNoteTitleTimeStyle--}
```
public static TextStyle getDefaultMsOneNoteTitleTimeStyle()
```


获取 MS OneNote 中标题时间的默认样式。

**Returns:**
[TextStyle](../../com.aspose.note/textstyle)
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public String getHyperlinkAddress()
```


获取超链接地址。如果 [isHyperlink](../../com.aspose.note/textstyle\#isHyperlink--) 属性的值为 true，则必须设置。

**Returns:**
java.lang.String
### getLanguage() {#getLanguage--}
```
public Locale getLanguage()
```


获取文本的语言。

**Returns:**
java.util.Locale
### hashCode() {#hashCode--}
```
public int hashCode()
```


作为该类型的哈希函数。

**Returns:**
int - 该 `int`。
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


获取指示文本样式是否隐藏的值。

**Returns:**
boolean
### isHyperlink() {#isHyperlink--}
```
public boolean isHyperlink()
```


获取指示文本样式是否为超链接的值。

**Returns:**
boolean
### isMathFormatting() {#isMathFormatting--}
```
public boolean isMathFormatting()
```


获取或设置指示文本样式是否为数学格式的值。

**Returns:**
boolean
### setHidden(boolean value) {#setHidden-boolean-}
```
public TextStyle setHidden(boolean value)
```


设置指示文本样式是否隐藏的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

**Returns:**
[TextStyle](../../com.aspose.note/textstyle)
### setHyperlink(boolean value) {#setHyperlink-boolean-}
```
public TextStyle setHyperlink(boolean value)
```


设置指示文本样式是否为超链接的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

**Returns:**
[TextStyle](../../com.aspose.note/textstyle)
### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public TextStyle setHyperlinkAddress(String value)
```


设置超链接地址。如果 [isHyperlink](../../com.aspose.note/textstyle\#isHyperlink--) 属性的值为 true，则必须设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

**Returns:**
[TextStyle](../../com.aspose.note/textstyle)
### setLanguage(Locale value) {#setLanguage-java.util.Locale-}
```
public TextStyle setLanguage(Locale value)
```


设置文本的语言。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Locale |  |

**Returns:**
[TextStyle](../../com.aspose.note/textstyle)
### setMathFormatting(boolean value) {#setMathFormatting-boolean-}
```
public TextStyle setMathFormatting(boolean value)
```


设置一个值，指示文本样式是否为数学格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

**Returns:**
[TextStyle](../../com.aspose.note/textstyle)
