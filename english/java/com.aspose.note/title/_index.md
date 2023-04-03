---
title: Title
second_title: Aspose.Note for Java API Reference
description: Represents a title.
type: docs
weight: 84
url: /java/com.aspose.note/title/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT, [com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class Title extends CompositeNodeBase implements ICompositeNodeT<RichText>, IPageChildNode
```

Represents a title.
## Constructors

| Constructor | Description |
| --- | --- |
| [Title()](#Title--) | Initializes a new instance of the  Title  class. |
## Methods

| Method | Description |
| --- | --- |
| [isComposite()](#isComposite--) | Gets a value indicating whether this node is composite. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Gets or sets the last modified time. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Gets or sets the last modified time. |
| [getTitleText()](#getTitleText--) | Gets or sets the text of the title. |
| [setTitleText(RichText value)](#setTitleText-com.aspose.note.RichText-) | Gets or sets the text of the title. |
| [getTitleDate()](#getTitleDate--) | Gets or sets a string representation of the date in the title. |
| [setTitleDate(RichText value)](#setTitleDate-com.aspose.note.RichText-) | Gets or sets a string representation of the date in the title. |
| [getTitleTime()](#getTitleTime--) | Gets or sets a string representation of the time in the title. |
| [setTitleTime(RichText value)](#setTitleTime-com.aspose.note.RichText-) | Gets or sets a string representation of the time in the title. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Gets or sets the horizontal offset. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Gets or sets the horizontal offset. |
| [getVerticalOffset()](#getVerticalOffset--) | Gets or sets the vertical offset. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Gets or sets the vertical offset. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepts the visitor of the node. |
| [getChildNodes(int type)](#getChildNodes-int-) |  |
| [<T1>getChildNodes(Class<T1> typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Get all child nodes by the node type. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through child nodes of the [Title](../../com.aspose.note/title). |
### Title() {#Title--}
```
public Title()
```


Initializes a new instance of the  Title  class.

### isComposite() {#isComposite--}
```
public boolean isComposite()
```


Gets a value indicating whether this node is composite. If true the node can have child nodes.

**Returns:**
boolean
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Gets or sets the last modified time.

**Returns:**
java.util.Date
### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Gets or sets the last modified time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date |  |

### getTitleText() {#getTitleText--}
```
public RichText getTitleText()
```


Gets or sets the text of the title.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### setTitleText(RichText value) {#setTitleText-com.aspose.note.RichText-}
```
public final void setTitleText(RichText value)
```


Gets or sets the text of the title.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### getTitleDate() {#getTitleDate--}
```
public final RichText getTitleDate()
```


Gets or sets a string representation of the date in the title.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### setTitleDate(RichText value) {#setTitleDate-com.aspose.note.RichText-}
```
public final void setTitleDate(RichText value)
```


Gets or sets a string representation of the date in the title.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### getTitleTime() {#getTitleTime--}
```
public final RichText getTitleTime()
```


Gets or sets a string representation of the time in the title.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### setTitleTime(RichText value) {#setTitleTime-com.aspose.note.RichText-}
```
public final void setTitleTime(RichText value)
```


Gets or sets a string representation of the time in the title.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### getHorizontalOffset() {#getHorizontalOffset--}
```
public final float getHorizontalOffset()
```


Gets or sets the horizontal offset.

**Returns:**
float
### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public final void setHorizontalOffset(float value)
```


Gets or sets the horizontal offset.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |

### getVerticalOffset() {#getVerticalOffset--}
```
public final float getVerticalOffset()
```


Gets or sets the vertical offset.

**Returns:**
float
### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public final void setVerticalOffset(float value)
```


Gets or sets the vertical offset.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepts the visitor of the node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | The object of a class derived from the  DocumentVisitor . |

### getChildNodes(int type) {#getChildNodes-int-}
```
public List<INode> getChildNodes(int type)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int |  |

**Returns:**
java.util.List<com.aspose.note.INode>
### <T1>getChildNodes(Class<T1> typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Get all child nodes by the node type.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| typeParameterClass | java.lang.Class<T1> |  |

**Returns:**
java.util.List<T1> - A list of child nodes.

 T1 : The type of elements in the returned list.
### iterator() {#iterator--}
```
public final System.Collections.Generic.IGenericEnumerator<RichText> iterator()
```


Returns an enumerator that iterates through child nodes of the [Title](../../com.aspose.note/title).

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator<com.aspose.note.RichText> - The IEnumerator.
