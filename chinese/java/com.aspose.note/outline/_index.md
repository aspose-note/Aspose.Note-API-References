---
title: "大纲"
second_title: "Aspose.Note for Java API 参考"
description: "表示大纲。"
type: docs
weight: 66
url: /zh/java/com.aspose.note/outline/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class Outline extends IndentatedNode<IOutlineChildNode,Outline> implements IPageChildNode
```

表示大纲。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Outline()](#Outline--) | 初始化一个新的 [Outline](../../com.aspose.note/outline) 类的实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | 接受节点的访问者。 |
| [getDescendantsCannotBeMoved()](#getDescendantsCannotBeMoved--) | 获取大纲的后代是否可以移动。 |
| [getHorizontalOffset()](#getHorizontalOffset--) | 获取或设置水平偏移。 |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
| [getLastModifiedTime()](#getLastModifiedTime--) | 获取或设置最后修改时间。 |
| [getMaxHeight()](#getMaxHeight--) | 获取或设置最大高度。 |
| [getMaxWidth()](#getMaxWidth--) | 获取或设置最大宽度。 |
| [getMinWidth()](#getMinWidth--) | 获取或设置最小宽度。 |
| [getReservedWidth()](#getReservedWidth--) | 获取或设置保留宽度。 |
| [getVerticalOffset()](#getVerticalOffset--) | 获取或设置垂直偏移。 |
| [setDescendantsCannotBeMoved(boolean value)](#setDescendantsCannotBeMoved-boolean-) | 获取大纲的后代是否可以移动。 |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | 获取或设置水平偏移。 |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 获取或设置最后修改时间。 |
| [setMaxHeight(float value)](#setMaxHeight-float-) | 获取或设置最大高度。 |
| [setMaxWidth(float value)](#setMaxWidth-float-) | 获取或设置最大宽度。 |
| [setMinWidth(float value)](#setMinWidth-float-) | 获取或设置最小宽度。 |
| [setReservedWidth(float value)](#setReservedWidth-float-) | 获取或设置保留宽度。 |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | 获取或设置垂直偏移。 |
### Outline() {#Outline--}
```
public Outline()
```


初始化一个新的 [Outline](../../com.aspose.note/outline) 类的实例。

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


接受节点的访问者。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | 从 `DocumentVisitor` 派生的类的对象。 |

### getDescendantsCannotBeMoved() {#getDescendantsCannotBeMoved--}
```
public boolean getDescendantsCannotBeMoved()
```


获取大纲的后代是否可以移动。

**Returns:**
boolean
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


获取或设置水平偏移。

**Returns:**
float
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
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


获取或设置最大高度。

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


获取或设置最大宽度。

**Returns:**
float
### getMinWidth() {#getMinWidth--}
```
public float getMinWidth()
```


获取或设置最小宽度。

**Returns:**
float
### getReservedWidth() {#getReservedWidth--}
```
public float getReservedWidth()
```


获取或设置保留宽度。

**Returns:**
float
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


获取或设置垂直偏移。

**Returns:**
float
### setDescendantsCannotBeMoved(boolean value) {#setDescendantsCannotBeMoved-boolean-}
```
public void setDescendantsCannotBeMoved(boolean value)
```


获取大纲的后代是否可以移动。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
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

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


获取或设置最大高度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | float |  |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


获取或设置最大宽度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | float |  |

### setMinWidth(float value) {#setMinWidth-float-}
```
public void setMinWidth(float value)
```


获取或设置最小宽度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | float |  |

### setReservedWidth(float value) {#setReservedWidth-float-}
```
public void setReservedWidth(float value)
```


获取或设置保留宽度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | float |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


获取或设置垂直偏移。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | float |  |

