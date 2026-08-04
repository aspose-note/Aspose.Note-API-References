---
title: OutlineElement
second_title: Aspose.Note for Java API Reference
description: Represents a OutlineElement.
type: docs
weight: 67
url: /java/com.aspose.note/outlineelement/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IOutlineChildNode](../../com.aspose.note/ioutlinechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode)
```
public final class OutlineElement extends IndentatedNode<IOutlineElementChildNode,OutlineElement> implements IOutlineChildNode, IOutlineElementChildNode
```

Represents a OutlineElement.
## Constructors

| Constructor | Description |
| --- | --- |
| [OutlineElement()](#OutlineElement--) | Initializes a new instance of the  OutlineElement  class. |
## Methods

| Method | Description |
| --- | --- |
| [<T1>appendChildFirst(T1 newChild)](#-T1-appendChildFirst-T1-) | Adds the node to the front of the list of child nodes for this node. |
| [<T1>appendChildLast(T1 newChild)](#-T1-appendChildLast-T1-) | Adds the node to the end of the list of child nodes for this node. |
| [<T1>getChildNodes(Class<T1> typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Get all child nodes by the node type. |
| [<T1>insertChild(int i, T1 newChild)](#-T1-insertChild-int-T1-) | Inserts the node to the specified position in the list of child nodes for this node. |
| [<T1>removeChild(T1 oldChild)](#-T1-removeChild-T1-) | Removes the child node. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepts the visitor of the node. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthorMostRecent()](#getAuthorMostRecent--) | Gets the most recent author of an outline element. |
| [getAuthorOriginal()](#getAuthorOriginal--) | Gets the original author of an outline element. |
| [getClass()](#getClass--) |  |
| [getCreationTime()](#getCreationTime--) | Gets or sets the creation time. |
| [getDocument()](#getDocument--) | Gets the document of the node. |
| [getFirstChild()](#getFirstChild--) | Gets the first child node of this node. |
| [getIndentPosition()](#getIndentPosition--) | Gets or sets the indent position. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) | Gets the amount of items to sum up in RgOutlineIndentDistance array to get indent size. |
| [getLastChild()](#getLastChild--) | Gets the last child node of this node. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Gets or sets the last modified time. |
| [getNextSibling()](#getNextSibling--) | Gets the next node at the same node tree level. |
| [getNodeId()](#getNodeId--) | Gets the node's ID. |
| [getNodeType()](#getNodeType--) | Gets the node type. |
| [getNumberList()](#getNumberList--) | Gets or sets the style for the numbered list header. |
| [getParentNode()](#getParentNode--) | Gets the parent node. |
| [getPreviousSibling()](#getPreviousSibling--) | Gets the previous node at the same node tree level. |
| [hashCode()](#hashCode--) |  |
| [insertChildrenRange(int i, T[] newChildren)](#insertChildrenRange-int-T...-) | Inserts the node's sequence starting from specified position in the list of child nodes for this node. |
| [insertChildrenRange(int i, Iterable<T> newChildren)](#insertChildrenRange-int-java.lang.Iterable-T--) | Inserts the node's sequence starting from specified position in the list of child nodes for this node. |
| [isComposite()](#isComposite--) | Checks whether the node is composite. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through child nodes of the  CompositeNode\{T\} . |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Gets or sets the creation time. |
| [setIndentPosition(byte value)](#setIndentPosition-byte-) | Gets or sets the indent position. |
| [setIndentPosition(int value)](#setIndentPosition-int-) |  |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Gets or sets the last modified time. |
| [setNumberList(NumberList value)](#setNumberList-com.aspose.note.NumberList-) | Gets or sets the style for the numbered list header. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### OutlineElement() {#OutlineElement--}
```
public OutlineElement()
```


Initializes a new instance of the  OutlineElement  class.

### <T1>appendChildFirst(T1 newChild) {#-T1-appendChildFirst-T1-}
```
public T1 <T1>appendChildFirst(T1 newChild)
```


Adds the node to the front of the list of child nodes for this node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| newChild | T1 | The node to add. |

**Returns:**
T1 - The added node.
### <T1>appendChildLast(T1 newChild) {#-T1-appendChildLast-T1-}
```
public T1 <T1>appendChildLast(T1 newChild)
```


Adds the node to the end of the list of child nodes for this node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| newChild | T1 | The node to add. |

**Returns:**
T1 - The added node.
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
### <T1>insertChild(int i, T1 newChild) {#-T1-insertChild-int-T1-}
```
public T1 <T1>insertChild(int i, T1 newChild)
```


Inserts the node to the specified position in the list of child nodes for this node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| i | int | Position to insert |
| newChild | T1 | The node to insert. |

**Returns:**
T1 - The added node.
### <T1>removeChild(T1 oldChild) {#-T1-removeChild-T1-}
```
public T1 <T1>removeChild(T1 oldChild)
```


Removes the child node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| oldChild | T1 | The node to remove. |

**Returns:**
T1 - The removed node.
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
### getAuthorMostRecent() {#getAuthorMostRecent--}
```
public final String getAuthorMostRecent()
```


Gets the most recent author of an outline element.

Value: The author most recent.

**Returns:**
java.lang.String
### getAuthorOriginal() {#getAuthorOriginal--}
```
public final String getAuthorOriginal()
```


Gets the original author of an outline element.

Value: The author original.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Gets or sets the creation time.

**Returns:**
java.util.Date
### getDocument() {#getDocument--}
```
public Document getDocument()
```


Gets the document of the node.

Value: The document.

**Returns:**
[Document](../../com.aspose.note/document)
### getFirstChild() {#getFirstChild--}
```
public T getFirstChild()
```


Gets the first child node of this node.

**Returns:**
T
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
### getLastChild() {#getLastChild--}
```
public T getLastChild()
```


Gets the last child node of this node.

**Returns:**
T
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
### getNumberList() {#getNumberList--}
```
public NumberList getNumberList()
```


Gets or sets the style for the numbered list header.

**Returns:**
[NumberList](../../com.aspose.note/numberlist)
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
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### insertChildrenRange(int i, T[] newChildren) {#insertChildrenRange-int-T...-}
```
public final void insertChildrenRange(int i, T[] newChildren)
```


Inserts the node's sequence starting from specified position in the list of child nodes for this node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| i | int | Position to insert |
| newChildren | T[] | The sequence of nodes to be inserted. |

### insertChildrenRange(int i, Iterable<T> newChildren) {#insertChildrenRange-int-java.lang.Iterable-T--}
```
public final void insertChildrenRange(int i, Iterable<T> newChildren)
```


Inserts the node's sequence starting from specified position in the list of child nodes for this node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| i | int | Position to insert |
| newChildren | java.lang.Iterable<T> | The sequence of nodes to be inserted. |

### isComposite() {#isComposite--}
```
public final boolean isComposite()
```


Checks whether the node is composite. If true then the node can have child nodes.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<T> iterator()
```


Returns an enumerator that iterates through child nodes of the  CompositeNode\{T\} .

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator<T> - A  T:IEnumerator1  for the  CompositeNode\{T\} .
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Gets or sets the creation time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date |  |

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
### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Gets or sets the last modified time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date |  |

### setNumberList(NumberList value) {#setNumberList-com.aspose.note.NumberList-}
```
public void setNumberList(NumberList value)
```


Gets or sets the style for the numbered list header.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NumberList](../../com.aspose.note/numberlist) |  |

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

