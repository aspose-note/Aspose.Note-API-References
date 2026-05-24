---
title: "RichText"
second_title: "Aspose.Note for Java API 参考"
description: "表示富文本。"
type: docs
weight: 82
url: /zh/java/com.aspose.note/richtext/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class RichText extends Node implements IOutlineElementChildNode, ITaggable, System.Collections.Generic.IGenericEnumerable<Character>
```

表示富文本。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [RichText()](#RichText--) | 初始化 [RichText](../../com.aspose.note/richtext) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | 接受节点的访问者。 |
| [append(String value)](#append-java.lang.String-) | 向最后的文本范围添加字符串。 |
| [append(String value, TextStyle style)](#append-java.lang.String-com.aspose.note.TextStyle-) | 在末尾添加字符串。 |
| [appendFront(String value)](#appendFront-java.lang.String-) | 在第一个文本范围的前面添加字符串。 |
| [appendFront(String value, TextStyle style)](#appendFront-java.lang.String-com.aspose.note.TextStyle-) | 在前面添加字符串。 |
| [clear()](#clear--) | 清除此实例的内容。 |
| [getAlignment()](#getAlignment--) | 获取对齐方式。 |
| [getLastModifiedTime()](#getLastModifiedTime--) | 获取最后修改时间。 |
| [getLength()](#getLength--) |  |
| [getLineSpacing()](#getLineSpacing--) | 获取行间距。 |
| [getParagraphStyle()](#getParagraphStyle--) | 获取段落样式。 |
| [getSpaceAfter()](#getSpaceAfter--) | 获取后面的最小间距。 |
| [getSpaceBefore()](#getSpaceBefore--) | 获取前面的最小间距。 |
| [getStyles()](#getStyles--) | 获取样式。 |
| [getTags()](#getTags--) | 获取段落的所有标签列表。 |
| [getText()](#getText--) | 获取文本。 |
| [getTextRuns()](#getTextRuns--) |  |
| [indexOf(char value)](#indexOf-char-) | 返回此字符串中指定 Unicode 字符首次出现的零基索引。 |
| [indexOf(char value, int startIndex)](#indexOf-char-int-) | 返回此字符串中指定 Unicode 字符首次出现的零基索引。 |
| [indexOf(char value, int startIndex, int count)](#indexOf-char-int-int-) | 返回此实例中指定字符首次出现的零基索引。 |
| [indexOf(String value)](#indexOf-java.lang.String-) | 返回此实例中指定字符串首次出现的零基索引。 |
| [indexOf(String value, int startIndex)](#indexOf-java.lang.String-int-) | 返回此实例中指定字符串首次出现的零基索引。 |
| [indexOf(String value, int startIndex, int count)](#indexOf-java.lang.String-int-int-) | 返回此实例中指定字符串首次出现的零基索引。 |
| [indexOf(String value, int startIndex, int count, short comparisonType)](#indexOf-java.lang.String-int-int-short-) | 返回当前实例中指定字符串首次出现的零基索引。 |
| [indexOf(String value, short comparisonType)](#indexOf-java.lang.String-short-) | 返回当前实例中指定字符串首次出现的零基索引。 |
| [indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)](#indexOf-Rename-Namesake-java.lang.String-int-short-) | 返回当前实例中指定字符串首次出现的零基索引。 |
| [insert(int startIndex, String value)](#insert-int-java.lang.String-) | 在此实例的指定索引位置插入指定字符串。 |
| [insert(int startIndex, String value, TextStyle style)](#insert-int-java.lang.String-com.aspose.note.TextStyle-) | 在此实例的指定索引位置插入带有指定样式的指定字符串。 |
| [iterator()](#iterator--) |  |
| [remove(int startIndex)](#remove-int-) | 从指定位置开始，删除当前实例中一直到最后位置的所有字符。 |
| [remove(int startIndex, int count)](#remove-int-int-) | 从指定位置开始，删除当前实例中指定数量的字符。 |
| [replace(char oldChar, char newChar)](#replace-char-char-) | 将此实例中所有指定 Unicode 字符的出现替换为另一个指定的 Unicode 字符。 |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | 将当前实例中所有指定字符串的出现替换为另一个指定字符串。 |
| [replace(String oldValue, String newValue, TextStyle style)](#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-) | 将当前实例中所有指定字符串的出现替换为另一个指定样式的指定字符串。 |
| [setAlignment(int value)](#setAlignment-int-) | 设置对齐方式。 |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 设置最后修改时间。 |
| [setLineSpacing(float value)](#setLineSpacing-float-) |  |
| [setLineSpacing(Float value)](#setLineSpacing-java.lang.Float-) | 设置行间距。 |
| [setParagraphStyle(ParagraphStyle value)](#setParagraphStyle-com.aspose.note.ParagraphStyle-) | 设置段落样式。 |
| [setSpaceAfter(float value)](#setSpaceAfter-float-) |  |
| [setSpaceAfter(Float value)](#setSpaceAfter-java.lang.Float-) | 设置后面的最小间距。 |
| [setSpaceBefore(float value)](#setSpaceBefore-float-) |  |
| [setSpaceBefore(Float value)](#setSpaceBefore-java.lang.Float-) | 设置之前的最小空间量。 |
| [setText(String value)](#setText-java.lang.String-) | 设置文本。 |
| [trim()](#trim--) | 删除所有前导和尾随的空白字符。 |
| [trim(char trimChar)](#trim-char-) | 删除所有前导和尾随的字符实例。 |
| [trim(char[] trimChars)](#trim-char...-) | 删除数组中指定的一组字符的所有前导和尾随出现。 |
| [trimEnd()](#trimEnd--) | 删除所有尾随的空白字符。 |
| [trimEnd(char trimChar)](#trimEnd-char-) | 删除字符的所有尾随出现。 |
| [trimEnd(char[] trimChars)](#trimEnd-char...-) | 删除数组中指定的一组字符的所有尾随出现。 |
| [trimStart()](#trimStart--) | 删除所有前导的空白字符。 |
| [trimStart(char trimChar)](#trimStart-char-) | 删除指定字符的所有前导出现。 |
| [trimStart(char[] trimChars)](#trimStart-char...-) | 删除数组中指定的一组字符的所有前导出现。 |
### RichText() {#RichText--}
```
public RichText()
```


初始化 [RichText](../../com.aspose.note/richtext) 类的新实例。

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


接受节点的访问者。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | 从 [DocumentVisitor](../../com.aspose.note/documentvisitor) 派生的类的对象。 |

### append(String value) {#append-java.lang.String-}
```
public RichText append(String value)
```


向最后的文本范围添加字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 添加的值。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### append(String value, TextStyle style) {#append-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText append(String value, TextStyle style)
```


在末尾添加字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 添加的值。 |
| style | [TextStyle](../../com.aspose.note/textstyle) | 添加字符串的样式。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value) {#appendFront-java.lang.String-}
```
public RichText appendFront(String value)
```


在第一个文本范围的前面添加字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 添加的值。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value, TextStyle style) {#appendFront-java.lang.String-com.aspose.note.TextStyle-}
```
public RichText appendFront(String value, TextStyle style)
```


在前面添加字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 添加的值。 |
| style | [TextStyle](../../com.aspose.note/textstyle) | 添加字符串的样式。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### clear() {#clear--}
```
public final RichText clear()
```


清除此实例的内容。

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


获取对齐方式。

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


获取最后修改时间。

**Returns:**
java.util.Date
### getLength() {#getLength--}
```
public final int getLength()
```




**Returns:**
int
### getLineSpacing() {#getLineSpacing--}
```
public Float getLineSpacing()
```


获取行间距。

**Returns:**
java.lang.Float
### getParagraphStyle() {#getParagraphStyle--}
```
public final ParagraphStyle getParagraphStyle()
```


获取段落样式。如果在 [getStyles](../../com.aspose.note/richtext\#getStyles) 集合中没有匹配的 TextStyle 对象，或者此对象未指定所需设置，则使用这些设置。

**Returns:**
[ParagraphStyle](../../com.aspose.note/paragraphstyle)
### getSpaceAfter() {#getSpaceAfter--}
```
public Float getSpaceAfter()
```


获取后面的最小间距。

**Returns:**
java.lang.Float
### getSpaceBefore() {#getSpaceBefore--}
```
public Float getSpaceBefore()
```


获取前面的最小间距。

**Returns:**
java.lang.Float
### getStyles() {#getStyles--}
```
public System.Collections.Generic.IGenericEnumerable<TextStyle> getStyles()
```


获取样式。

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.TextStyle&gt;
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


获取段落的所有标签列表。

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public final String getText()
```


获取文本。字符串不得包含值为 10（换行）的任何字符。

**Returns:**
java.lang.String
### getTextRuns() {#getTextRuns--}
```
public final System.Collections.Generic.IGenericEnumerable<TextRun> getTextRuns()
```




**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.TextRun&gt;
### indexOf(char value) {#indexOf-char-}
```
public final int indexOf(char value)
```


返回此字符串中指定 Unicode 字符首次出现的零基索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | char | 该值。 |

**Returns:**
int - 该 `int`。
### indexOf(char value, int startIndex) {#indexOf-char-int-}
```
public final int indexOf(char value, int startIndex)
```


返回此字符串中指定 Unicode 字符首次出现的零基索引。搜索从指定的字符位置开始。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | char | 该值。 |
| startIndex | int | 起始搜索位置 |

**Returns:**
int - 该 `int`。
### indexOf(char value, int startIndex, int count) {#indexOf-char-int-int-}
```
public final int indexOf(char value, int startIndex, int count)
```


返回此实例中指定字符首次出现的零基索引。搜索从指定的字符位置开始，并检查指定数量的字符位置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | char | 该值。 |
| startIndex | int | 起始搜索位置 |
| count | int | 计数。 |

**Returns:**
int - 该 `int`。
### indexOf(String value) {#indexOf-java.lang.String-}
```
public final int indexOf(String value)
```


返回此实例中指定字符串首次出现的零基索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 该值。 |

**Returns:**
int - 该 `int`。
### indexOf(String value, int startIndex) {#indexOf-java.lang.String-int-}
```
public final int indexOf(String value, int startIndex)
```


返回此实例中指定字符串首次出现的零基索引。搜索从指定的字符位置开始。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 该值。 |
| startIndex | int | 起始搜索位置 |

**Returns:**
int - 该 `int`。
### indexOf(String value, int startIndex, int count) {#indexOf-java.lang.String-int-int-}
```
public final int indexOf(String value, int startIndex, int count)
```


返回此实例中指定字符串首次出现的零基索引。搜索从指定的字符位置开始，并检查指定数量的字符位置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 该值。 |
| startIndex | int | 起始搜索位置 |
| count | int | 计数。 |

**Returns:**
int - 该 `int`。
### indexOf(String value, int startIndex, int count, short comparisonType) {#indexOf-java.lang.String-int-int-short-}
```
public final int indexOf(String value, int startIndex, int count, short comparisonType)
```


返回当前实例中指定字符串首次出现的零基索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 该值。 |
| startIndex | int | 起始搜索位置 |
| count | int | 计数。 |
| comparisonType | short | 用于指定字符串的搜索类型 |

**Returns:**
int - 该 `int`。
### indexOf(String value, short comparisonType) {#indexOf-java.lang.String-short-}
```
public final int indexOf(String value, short comparisonType)
```


返回当前实例中指定字符串首次出现的零基索引。参数指定用于指定字符串的搜索类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 该值。 |
| comparisonType | short | 用于指定字符串的搜索类型 |

**Returns:**
int - 该 `int`。
### indexOf_Rename_Namesake(String value, int startIndex, short comparisonType) {#indexOf-Rename-Namesake-java.lang.String-int-short-}
```
public final int indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)
```


返回当前实例中指定字符串首次出现的零基索引。参数指定当前字符串的起始搜索位置以及用于指定字符串的搜索类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 该值。 |
| startIndex | int | 起始搜索位置 |
| comparisonType | short | 用于指定字符串的搜索类型 |

**Returns:**
int - 该 `int`。
### insert(int startIndex, String value) {#insert-int-java.lang.String-}
```
public final RichText insert(int startIndex, String value)
```


在此实例的指定索引位置插入指定字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startIndex | int | 起始索引。 |
| 值 | java.lang.String | 该值。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### insert(int startIndex, String value, TextStyle style) {#insert-int-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText insert(int startIndex, String value, TextStyle style)
```


在此实例的指定索引位置插入带有指定样式的指定字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startIndex | int | 起始索引。 |
| 值 | java.lang.String | 该值。 |
| style | [TextStyle](../../com.aspose.note/textstyle) | 样式。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<Character> iterator()
```




**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;java.lang.Character&gt;
### remove(int startIndex) {#remove-int-}
```
public final RichText remove(int startIndex)
```


从指定位置开始，删除当前实例中一直到最后位置的所有字符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startIndex | int | 起始索引。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### remove(int startIndex, int count) {#remove-int-int-}
```
public final RichText remove(int startIndex, int count)
```


从指定位置开始，删除当前实例中指定数量的字符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startIndex | int | 起始索引。 |
| count | int | 计数。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public final RichText replace(char oldChar, char newChar)
```


将此实例中所有指定 Unicode 字符的出现替换为另一个指定的 Unicode 字符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| oldChar | char | 旧字符。 |
| newChar | char | 新字符。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public final RichText replace(String oldValue, String newValue)
```


将当前实例中所有指定字符串的出现替换为另一个指定字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| oldValue | java.lang.String | 旧值。 |
| newValue | java.lang.String | 新值。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue, TextStyle style) {#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText replace(String oldValue, String newValue, TextStyle style)
```


将当前实例中所有指定字符串的出现替换为另一个指定样式的指定字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| oldValue | java.lang.String | 旧值。 |
| newValue | java.lang.String | 新值。 |
| style | [TextStyle](../../com.aspose.note/textstyle) | 新值的样式。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


设置对齐方式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


设置最后修改时间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date |  |

### setLineSpacing(float value) {#setLineSpacing-float-}
```
public void setLineSpacing(float value)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | float |  |

### setLineSpacing(Float value) {#setLineSpacing-java.lang.Float-}
```
public void setLineSpacing(Float value)
```


设置行间距。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Float |  |

### setParagraphStyle(ParagraphStyle value) {#setParagraphStyle-com.aspose.note.ParagraphStyle-}
```
public final void setParagraphStyle(ParagraphStyle value)
```


设置段落样式。如果在[getStyles](../../com.aspose.note/richtext\#getStyles)集合中没有匹配的 TextStyle 对象，或者此对象未指定所需设置，则使用这些设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [ParagraphStyle](../../com.aspose.note/paragraphstyle) |  |

### setSpaceAfter(float value) {#setSpaceAfter-float-}
```
public void setSpaceAfter(float value)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | float |  |

### setSpaceAfter(Float value) {#setSpaceAfter-java.lang.Float-}
```
public void setSpaceAfter(Float value)
```


设置后面的最小间距。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Float |  |

### setSpaceBefore(float value) {#setSpaceBefore-float-}
```
public void setSpaceBefore(float value)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | float |  |

### setSpaceBefore(Float value) {#setSpaceBefore-java.lang.Float-}
```
public void setSpaceBefore(Float value)
```


设置之前的最小空间量。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Float |  |

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


设置文本。字符串不得包含值为 10 的字符（换行符）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### trim() {#trim--}
```
public final RichText trim()
```


删除所有前导和尾随的空白字符。

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char trimChar) {#trim-char-}
```
public final RichText trim(char trimChar)
```


删除所有前导和尾随的字符实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| trimChar | char | 修剪字符。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char[] trimChars) {#trim-char...-}
```
public final RichText trim(char[] trimChars)
```


删除数组中指定的一组字符的所有前导和尾随出现。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| trimChars | char[] | 修剪字符。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd() {#trimEnd--}
```
public final RichText trimEnd()
```


删除所有尾随的空白字符。

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char trimChar) {#trimEnd-char-}
```
public final RichText trimEnd(char trimChar)
```


删除字符的所有尾随出现。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| trimChar | char | 修剪字符。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char[] trimChars) {#trimEnd-char...-}
```
public final RichText trimEnd(char[] trimChars)
```


删除数组中指定的一组字符的所有尾随出现。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| trimChars | char[] | 修剪字符。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart() {#trimStart--}
```
public final RichText trimStart()
```


删除所有前导的空白字符。

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char trimChar) {#trimStart-char-}
```
public final RichText trimStart(char trimChar)
```


删除指定字符的所有前导出现。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| trimChar | char | 修剪字符。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char[] trimChars) {#trimStart-char...-}
```
public final RichText trimStart(char[] trimChars)
```


删除数组中指定的一组字符的所有前导出现。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| trimChars | char[] | 修剪字符。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
