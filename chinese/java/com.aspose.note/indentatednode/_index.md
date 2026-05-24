---
title: "IndentatedNode"
second_title: "Aspose.Note for Java API 参考"
description: "用于子节点具有相对缩进的节点的基础类。"
type: docs
weight: 37
url: /zh/java/com.aspose.note/indentatednode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
com.aspose.note.IIndentatedNodeExtended
```
public class IndentatedNode<T,Self> extends CompositeNode<T> implements IIndentatedNodeExtended
```

用于子节点具有相对缩进的节点的基础类。

`T`：复合节点中元素的类型。

T :
Self :
## 方法

| 方法 | 描述 |
| --- | --- |
| [getIndentPosition()](#getIndentPosition--) | 获取或设置缩进位置。 |
| [getInternalIndentPosition()](#getInternalIndentPosition--) | 获取在 RgOutlineIndentDistance 数组中求和的项数，以获得缩进大小。 |
| [setIndentPosition(byte value)](#setIndentPosition-byte-) | 获取或设置缩进位置。 |
| [setIndentPosition(int value)](#setIndentPosition-int-) |  |
### getIndentPosition() {#getIndentPosition--}
```
public final byte getIndentPosition()
```


获取或设置缩进位置。

**Returns:**
byte
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


获取在 RgOutlineIndentDistance 数组中求和的项数，以获得缩进大小。

**Returns:**
int
### setIndentPosition(byte value) {#setIndentPosition-byte-}
```
public final Self setIndentPosition(byte value)
```


获取或设置缩进位置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | byte |  |

**Returns:**
Self
### setIndentPosition(int value) {#setIndentPosition-int-}
```
public final Self setIndentPosition(int value)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

**Returns:**
Self
