---
title: IndentatedNode
second_title: Aspose.Note for Java API Reference
description: The base class for nodes with relative indentation for child nodes.
type: docs
weight: 37
url: /java/com.aspose.note/indentatednode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
com.aspose.note.IIndentatedNodeExtended
```
public class IndentatedNode<T,Self> extends CompositeNode<T> implements IIndentatedNodeExtended
```

The base class for nodes with relative indentation for child nodes.

`T`: The type of elements in the composite node.

 T : 
 Self : 
## Methods

| Method | Description |
| --- | --- |
| [getIndentPosition()](#getIndentPosition--) | Gets or sets the indent position. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) | Gets the amount of items to sum up in RgOutlineIndentDistance array to get indent size. |
| [setIndentPosition(byte value)](#setIndentPosition-byte-) | Gets or sets the indent position. |
| [setIndentPosition(int value)](#setIndentPosition-int-) |  |
### getIndentPosition() {#getIndentPosition--}
```
public final byte getIndentPosition()
```


Gets or sets the indent position.

**Returns:**
byte
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


Gets the amount of items to sum up in RgOutlineIndentDistance array to get indent size.

**Returns:**
int
### setIndentPosition(byte value) {#setIndentPosition-byte-}
```
public final Self setIndentPosition(byte value)
```


Gets or sets the indent position.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte |  |

**Returns:**
Self
### setIndentPosition(int value) {#setIndentPosition-int-}
```
public final Self setIndentPosition(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

**Returns:**
Self
