---
title: "Title"
second_title: "Aspose.Note for Java API 参考"
description: "表示标题。"
type: docs
weight: 95
url: /zh/java/com.aspose.note/title/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT, [com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class Title extends CompositeNodeBase implements ICompositeNodeT<RichText>, IPageChildNode
```

表示标题。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Title()](#Title--) | 初始化 `Title` 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | 按节点类型获取所有子节点。 |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | 接受节点的访问者。 |
| [getChildNodes(int type)](#getChildNodes-int-) |  |
| [getHorizontalOffset()](#getHorizontalOffset--) | 获取或设置水平偏移。 |
| [getLastModifiedTime()](#getLastModifiedTime--) | 获取或设置最后修改时间。 |
| [getTitleDate()](#getTitleDate--) | 获取或设置标题中日期的字符串表示形式。 |
| [getTitleText()](#getTitleText--) | 获取或设置标题的文本。 |
| [getTitleTime()](#getTitleTime--) | 获取或设置标题中时间的字符串表示形式。 |
| [getVerticalOffset()](#getVerticalOffset--) | 获取或设置垂直偏移。 |
| [isComposite()](#isComposite--) | 获取指示此节点是否为复合节点的值。 |
| [iterator()](#iterator--) | 返回一个枚举器，用于遍历 [Title](../../com.aspose.note/title) 的子节点。 |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | 获取或设置水平偏移。 |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 获取或设置最后修改时间。 |
| [setTitleDate(RichText value)](#setTitleDate-com.aspose.note.RichText-) | 获取或设置标题中日期的字符串表示形式。 |
| [setTitleText(RichText value)](#setTitleText-com.aspose.note.RichText-) | 获取或设置标题的文本。 |
| [setTitleTime(RichText value)](#setTitleTime-com.aspose.note.RichText-) | 获取或设置标题中时间的字符串表示形式。 |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | 获取或设置垂直偏移。 |
### Title() {#Title--}
```
public Title()
```


初始化 `Title` 类的新实例。

### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


按节点类型获取所有子节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - 子节点的列表。

`T1`：返回列表中元素的类型。
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


接受节点的访问者。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | 从 `DocumentVisitor` 派生的类的对象。 |

### getChildNodes(int type) {#getChildNodes-int-}
```
public List<INode> getChildNodes(int type)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 类型 | int |  |

**Returns:**
java.util.List&lt;com.aspose.note.INode&gt;
### getHorizontalOffset() {#getHorizontalOffset--}
```
public final float getHorizontalOffset()
```


获取或设置水平偏移。

**Returns:**
float
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


获取或设置最后修改时间。

**Returns:**
java.util.Date
### getTitleDate() {#getTitleDate--}
```
public final RichText getTitleDate()
```


获取或设置标题中日期的字符串表示形式。

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getTitleText() {#getTitleText--}
```
public RichText getTitleText()
```


获取或设置标题的文本。

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getTitleTime() {#getTitleTime--}
```
public final RichText getTitleTime()
```


获取或设置标题中时间的字符串表示形式。

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getVerticalOffset() {#getVerticalOffset--}
```
public final float getVerticalOffset()
```


获取或设置垂直偏移。

**Returns:**
float
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


获取指示此节点是否为复合节点的值。如果为 true，则该节点可以拥有子节点。

**Returns:**
boolean
### iterator() {#iterator--}
```
public final System.Collections.Generic.IGenericEnumerator<RichText> iterator()
```


返回一个枚举器，用于遍历 [Title](../../com.aspose.note/title) 的子节点。

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.RichText&gt; - IEnumerator。
### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public final void setHorizontalOffset(float value)
```


获取或设置水平偏移。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | float |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


获取或设置最后修改时间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date |  |

### setTitleDate(RichText value) {#setTitleDate-com.aspose.note.RichText-}
```
public final void setTitleDate(RichText value)
```


获取或设置标题中日期的字符串表示形式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setTitleText(RichText value) {#setTitleText-com.aspose.note.RichText-}
```
public final void setTitleText(RichText value)
```


获取或设置标题的文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setTitleTime(RichText value) {#setTitleTime-com.aspose.note.RichText-}
```
public final void setTitleTime(RichText value)
```


获取或设置标题中时间的字符串表示形式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public final void setVerticalOffset(float value)
```


获取或设置垂直偏移。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | float |  |

