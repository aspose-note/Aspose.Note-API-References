---
title: Title
second_title: Aspose.Note for Java API Reference
description: Represents a title.
type: docs
weight: 95
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
| [<T1>getChildNodes(Class<T1> typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Get all child nodes by the node type. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepts the visitor of the node. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getChildNodes(int type)](#getChildNodes-int-) |  |
| [getClass()](#getClass--) |  |
| [getDocument()](#getDocument--) | Gets the document of the node. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Gets or sets the horizontal offset. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Gets or sets the last modified time. |
| [getNextSibling()](#getNextSibling--) | Gets the next node at the same node tree level. |
| [getNodeId()](#getNodeId--) | Gets the node's ID. |
| [getNodeType()](#getNodeType--) | Gets the node type. |
| [getParentNode()](#getParentNode--) | Gets the parent node. |
| [getPreviousSibling()](#getPreviousSibling--) | Gets the previous node at the same node tree level. |
| [getTitleDate()](#getTitleDate--) | Gets or sets a string representation of the date in the title. |
| [getTitleText()](#getTitleText--) | Gets or sets the text of the title. |
| [getTitleTime()](#getTitleTime--) | Gets or sets a string representation of the time in the title. |
| [getVerticalOffset()](#getVerticalOffset--) | Gets or sets the vertical offset. |
| [hashCode()](#hashCode--) |  |
| [isComposite()](#isComposite--) | Gets a value indicating whether this node is composite. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through child nodes of the [Title](../../com.aspose.note/title). |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Gets or sets the horizontal offset. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Gets or sets the last modified time. |
| [setTitleDate(RichText value)](#setTitleDate-com.aspose.note.RichText-) | Gets or sets a string representation of the date in the title. |
| [setTitleText(RichText value)](#setTitleText-com.aspose.note.RichText-) | Gets or sets the text of the title. |
| [setTitleTime(RichText value)](#setTitleTime-com.aspose.note.RichText-) | Gets or sets a string representation of the time in the title. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Gets or sets the vertical offset. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Title() {#Title--}
```
public Title()
```


Initializes a new instance of the  Title  class.

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
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepts the visitor of the node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | The object of a class derived from the  DocumentVisitor . |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDocument() {#getDocument--}
```
public Document getDocument()
```


Gets the document of the node.

Value: The document.

**Returns:**
[Document](../../com.aspose.note/document)
### getHorizontalOffset() {#getHorizontalOffset--}
```
public final float getHorizontalOffset()
```


Gets or sets the horizontal offset.

**Returns:**
float
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Gets or sets the last modified time.

**Returns:**
java.util.Date
### getNextSibling() {#getNextSibling--}
```
public INode getNextSibling()
```


Gets the next node at the same node tree level.

Value: The next sibling.

**Returns:**
[INode](../../com.aspose.note/inode)
### getNodeId() {#getNodeId--}
```
public ExtendedGuid getNodeId()
```


Gets the node's ID.

**Returns:**
[ExtendedGuid](../../com.aspose.note.revision.types/extendedguid)
### getNodeType() {#getNodeType--}
```
public int getNodeType()
```


Gets the node type.

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public ICompositeNode getParentNode()
```


Gets the parent node.

**Returns:**
[ICompositeNode](../../com.aspose.note/icompositenode)
### getPreviousSibling() {#getPreviousSibling--}
```
public INode getPreviousSibling()
```


Gets the previous node at the same node tree level.

Value: The previous sibling.

**Returns:**
[INode](../../com.aspose.note/inode)
### getTitleDate() {#getTitleDate--}
```
public final RichText getTitleDate()
```


Gets or sets a string representation of the date in the title.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getTitleText() {#getTitleText--}
```
public RichText getTitleText()
```


Gets or sets the text of the title.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getTitleTime() {#getTitleTime--}
```
public final RichText getTitleTime()
```


Gets or sets a string representation of the time in the title.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getVerticalOffset() {#getVerticalOffset--}
```
public final float getVerticalOffset()
```


Gets or sets the vertical offset.

**Returns:**
float
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


Gets a value indicating whether this node is composite. If true the node can have child nodes.

**Returns:**
boolean
### iterator() {#iterator--}
```
public final System.Collections.Generic.IGenericEnumerator<RichText> iterator()
```


Returns an enumerator that iterates through child nodes of the [Title](../../com.aspose.note/title).

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator<com.aspose.note.RichText> - The IEnumerator.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public final void setHorizontalOffset(float value)
```


Gets or sets the horizontal offset.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Gets or sets the last modified time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date |  |

### setTitleDate(RichText value) {#setTitleDate-com.aspose.note.RichText-}
```
public final void setTitleDate(RichText value)
```


Gets or sets a string representation of the date in the title.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setTitleText(RichText value) {#setTitleText-com.aspose.note.RichText-}
```
public final void setTitleText(RichText value)
```


Gets or sets the text of the title.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setTitleTime(RichText value) {#setTitleTime-com.aspose.note.RichText-}
```
public final void setTitleTime(RichText value)
```


Gets or sets a string representation of the time in the title.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public final void setVerticalOffset(float value)
```


Gets or sets the vertical offset.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final void wait(long arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

