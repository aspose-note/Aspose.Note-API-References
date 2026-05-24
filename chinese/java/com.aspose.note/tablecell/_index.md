---
title: "TableCell"
second_title: "Aspose.Note for Java API 参考"
description: "表示一个表格单元格。"
type: docs
weight: 88
url: /zh/java/com.aspose.note/tablecell/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode
```
public final class TableCell extends IndentatedNode<IOutlineChildNode,TableCell>
```

表示一个表格单元格。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [TableCell()](#TableCell--) | 初始化 `TableCell` 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | 接受节点的访问者。 |
| [getBackgroundColor()](#getBackgroundColor--) | 获取背景颜色。 |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
| [getLastModifiedTime()](#getLastModifiedTime--) | 获取或设置最后修改时间。 |
| [getMaxWidth()](#getMaxWidth--) | 获取最大宽度。 |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | 设置背景颜色。 |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 获取或设置最后修改时间。 |
### TableCell() {#TableCell--}
```
public TableCell()
```


初始化 `TableCell` 类的新实例。

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


接受节点的访问者。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | 从 `DocumentVisitor` 派生的类的对象。 |

### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


获取背景颜色。

**Returns:**
java.awt.Color
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


获取在 RgOutlineIndentDistance 数组中求和的项数，以获得缩进大小。

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


获取或设置最后修改时间。

**Returns:**
java.util.Date
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


获取最大宽度。

**Returns:**
float
### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public void setBackgroundColor(Color value)
```


设置背景颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.awt.Color |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


获取或设置最后修改时间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date |  |

