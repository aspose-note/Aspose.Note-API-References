---
title: InkDrawing
second_title: Aspose.Note for Java API Reference
description: Represents a ink node containing any drawn content.
type: docs
weight: 38
url: /java/com.aspose.note/inkdrawing/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.InkNode](../../com.aspose.note/inknode)

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class InkDrawing extends InkNode implements IPageChildNode
```

Represents a ink node containing any drawn content.
## Methods

| Method | Description |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepts the visitor of the node. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDocument()](#getDocument--) | Gets the document of the node. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Gets the horizontal offset. |
| [getNextSibling()](#getNextSibling--) | Gets the next node at the same node tree level. |
| [getNodeId()](#getNodeId--) | Gets the node's ID. |
| [getNodeType()](#getNodeType--) | Gets the node type. |
| [getParentNode()](#getParentNode--) | Gets the parent node. |
| [getPreviousSibling()](#getPreviousSibling--) | Gets the previous node at the same node tree level. |
| [getVerticalOffset()](#getVerticalOffset--) | Gets the vertical offset. |
| [hashCode()](#hashCode--) |  |
| [isComposite()](#isComposite--) | Gets a value indicating whether this node is composite. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Sets the horizontal offset. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Sets the vertical offset. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepts the visitor of the node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | The object of a class derived from the [DocumentVisitor](../../com.aspose.note/documentvisitor). |

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


Gets the horizontal offset.

**Returns:**
float
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
### getVerticalOffset() {#getVerticalOffset--}
```
public final float getVerticalOffset()
```


Gets the vertical offset.

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


Sets the horizontal offset.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public final void setVerticalOffset(float value)
```


Sets the vertical offset.

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

