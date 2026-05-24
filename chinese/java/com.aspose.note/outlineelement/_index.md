---
title: "OutlineElement"
second_title: "Aspose.Note for Java API 参考"
description: "表示一个 OutlineElement。"
type: docs
weight: 67
url: /zh/java/com.aspose.note/outlineelement/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IOutlineChildNode](../../com.aspose.note/ioutlinechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode)
```
public final class OutlineElement extends IndentatedNode<IOutlineElementChildNode,OutlineElement> implements IOutlineChildNode, IOutlineElementChildNode
```

表示一个 OutlineElement。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [OutlineElement()](#OutlineElement--) | 初始化 `OutlineElement` 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | 接受节点的访问者。 |
| [getAuthorMostRecent()](#getAuthorMostRecent--) | 获取大纲元素的最新作者。 |
| [getAuthorOriginal()](#getAuthorOriginal--) | 获取大纲元素的原始作者。 |
| [getCreationTime()](#getCreationTime--) | 获取或设置创建时间。 |
| [getLastModifiedTime()](#getLastModifiedTime--) | 获取或设置最后修改时间。 |
| [getNumberList()](#getNumberList--) | 获取或设置编号列表标题的样式。 |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | 获取或设置创建时间。 |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 获取或设置最后修改时间。 |
| [setNumberList(NumberList value)](#setNumberList-com.aspose.note.NumberList-) | 获取或设置编号列表标题的样式。 |
### OutlineElement() {#OutlineElement--}
```
public OutlineElement()
```


初始化 `OutlineElement` 类的新实例。

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


接受节点的访问者。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | 从 `DocumentVisitor` 派生的类的对象。 |

### getAuthorMostRecent() {#getAuthorMostRecent--}
```
public final String getAuthorMostRecent()
```


获取大纲元素的最新作者。

值：最新的作者。

**Returns:**
java.lang.String
### getAuthorOriginal() {#getAuthorOriginal--}
```
public final String getAuthorOriginal()
```


获取大纲元素的原始作者。

值：原始作者。

**Returns:**
java.lang.String
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


获取或设置创建时间。

**Returns:**
java.util.Date
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


获取或设置最后修改时间。

**Returns:**
java.util.Date
### getNumberList() {#getNumberList--}
```
public NumberList getNumberList()
```


获取或设置编号列表标题的样式。

**Returns:**
[NumberList](../../com.aspose.note/numberlist)
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


获取或设置创建时间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


获取或设置最后修改时间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date |  |

### setNumberList(NumberList value) {#setNumberList-com.aspose.note.NumberList-}
```
public void setNumberList(NumberList value)
```


获取或设置编号列表标题的样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [NumberList](../../com.aspose.note/numberlist) |  |

