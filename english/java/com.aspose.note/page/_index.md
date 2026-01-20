---
title: Page
second_title: Aspose.Note for Java API Reference
description: Represents a page.
type: docs
weight: 69
url: /java/com.aspose.note/page/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode
```
public final class Page extends CompositeNode<IPageChildNode>
```

Represents a page.
## Constructors

| Constructor | Description |
| --- | --- |
| [Page()](#Page--) | Initializes a new instance of the  Page  class. |
## Methods

| Method | Description |
| --- | --- |
| [<T1>appendChildFirst(T1 newChild)](#-T1-appendChildFirst-T1-) | Adds the node to the front of the list of child nodes for this node. |
| [<T1>appendChildLast(T1 newChild)](#-T1-appendChildLast-T1-) | Adds the node to the end of the list of child nodes for this node. |
| [<T1>getChildNodes(Class<T1> typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Get all child nodes by the node type. |
| [<T1>insertChild(int i, T1 newChild)](#-T1-insertChild-int-T1-) | Inserts the node to the specified position in the list of child nodes for this node. |
| [<T1>removeChild(T1 oldChild)](#-T1-removeChild-T1-) | Removes the child node. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepts the visitor of the node. |
| [deepClone()](#deepClone--) | Clones the page. |
| [deepClone(boolean cloneHistory)](#deepClone-boolean-) | Clones the page. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | Gets or sets the author. |
| [getBackgroundColor()](#getBackgroundColor--) | Gets or sets page's background color. |
| [getClass()](#getClass--) |  |
| [getCreationTime()](#getCreationTime--) | Gets or sets the creation time. |
| [getDocument()](#getDocument--) | Gets the document of the node. |
| [getFirstChild()](#getFirstChild--) | Gets the first child node of this node. |
| [getLastChild()](#getLastChild--) | Gets the last child node of this node. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Gets or sets the last modified time. |
| [getLevel()](#getLevel--) | Gets or sets the level. |
| [getMargin()](#getMargin--) | Gets or sets the margin. |
| [getNextSibling()](#getNextSibling--) | Gets the next node at the same node tree level. |
| [getNodeId()](#getNodeId--) | Gets the node's ID. |
| [getNodeType()](#getNodeType--) | Gets the node type. |
| [getPageContentRevisionSummary()](#getPageContentRevisionSummary--) | Gets or sets the revision summary for the page and it's child nodes. |
| [getPageLayoutSize()](#getPageLayoutSize--) | Gets page's layout size displayed in the editor. |
| [getParentNode()](#getParentNode--) | Gets the parent node. |
| [getPreviousSibling()](#getPreviousSibling--) | Gets the previous node at the same node tree level. |
| [getSizeType()](#getSizeType--) | Gets or sets the size type of a page. |
| [getTitle()](#getTitle--) | Gets or sets the title. |
| [hashCode()](#hashCode--) |  |
| [insertChildrenRange(int i, T[] newChildren)](#insertChildrenRange-int-T...-) | Inserts the node's sequence starting from specified position in the list of child nodes for this node. |
| [insertChildrenRange(int i, Iterable<T> newChildren)](#insertChildrenRange-int-java.lang.Iterable-T--) | Inserts the node's sequence starting from specified position in the list of child nodes for this node. |
| [isComposite()](#isComposite--) | Checks whether the node is composite. |
| [isConflictPage()](#isConflictPage--) | Gets or sets a value indicating whether this page is a conflict page. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through child nodes of the  CompositeNode\{T\} . |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Gets or sets the author. |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | Gets or sets page's background color. |
| [setConflictPage(boolean value)](#setConflictPage-boolean-) | Gets or sets a value indicating whether this page is a conflict page. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Gets or sets the creation time. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Gets or sets the last modified time. |
| [setLevel(byte value)](#setLevel-byte-) | Gets or sets the level. |
| [setMargin(Margins value)](#setMargin-com.aspose.note.Margins-) | Gets or sets the margin. |
| [setPageContentRevisionSummary(RevisionSummary value)](#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-) | Gets or sets the revision summary for the page and it's child nodes. |
| [setPageLayoutSize(Dimension2D value)](#setPageLayoutSize-java.awt.geom.Dimension2D-) | Sets page's layout size displayed in the editor. |
| [setSizeType(int value)](#setSizeType-int-) | Gets or sets the size type of a page. |
| [setTitle(Title value)](#setTitle-com.aspose.note.Title-) | Gets or sets the title. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Page() {#Page--}
```
public Page()
```


Initializes a new instance of the  Page  class.

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

### deepClone() {#deepClone--}
```
public final Page deepClone()
```


Clones the page.

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### deepClone(boolean cloneHistory) {#deepClone-boolean-}
```
public final Page deepClone(boolean cloneHistory)
```


Clones the page.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cloneHistory | boolean | Specifies if page's history should be cloned.. |

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
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
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Gets or sets the author.

**Returns:**
java.lang.String
### getBackgroundColor() {#getBackgroundColor--}
```
public final Color getBackgroundColor()
```


Gets or sets page's background color.

**Returns:**
java.awt.Color
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
### getLevel() {#getLevel--}
```
public byte getLevel()
```


Gets or sets the level.

**Returns:**
byte
### getMargin() {#getMargin--}
```
public Margins getMargin()
```


Gets or sets the margin.

**Returns:**
[Margins](../../com.aspose.note/margins)
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
### getPageContentRevisionSummary() {#getPageContentRevisionSummary--}
```
public RevisionSummary getPageContentRevisionSummary()
```


Gets or sets the revision summary for the page and it's child nodes.

**Returns:**
[RevisionSummary](../../com.aspose.note/revisionsummary)
### getPageLayoutSize() {#getPageLayoutSize--}
```
public final Dimension2D getPageLayoutSize()
```


Gets page's layout size displayed in the editor.

--------------------

This value is used by Microsoft OneNote application to display underlying page layout when document is opened. It doesn't affect printing and saving of the document anyway. When Page.SizeType property is set to PageSizeType.SizeByContent this property returns real size of the content.

**Returns:**
java.awt.geom.Dimension2D
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
### getSizeType() {#getSizeType--}
```
public final int getSizeType()
```


Gets or sets the size type of a page.

--------------------

By default, a page resizes automatically. The default value is [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent).

**Returns:**
int
### getTitle() {#getTitle--}
```
public Title getTitle()
```


Gets or sets the title.

Value: The  Title .

**Returns:**
[Title](../../com.aspose.note/title)
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
### isConflictPage() {#isConflictPage--}
```
public final boolean isConflictPage()
```


Gets or sets a value indicating whether this page is a conflict page.

--------------------

The conflict page arises when two users try to update the same content. In this case the changes of first user are written as usual. But changes of another user can't be merged. So just a copy of page is created and marked as conflict.

At this version the conflicts are resolved in favor of the first user's changes. So if document has conflict pages then they will be shown in history but they will be skipped on saving. It is possible to reset this flag to save this pages in history as usual ones.

Detailed sample of manipulating by conflict page can be found in the online documentation.

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




### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Gets or sets the author.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public final void setBackgroundColor(Color value)
```


Gets or sets page's background color.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.awt.Color |  |

### setConflictPage(boolean value) {#setConflictPage-boolean-}
```
public final void setConflictPage(boolean value)
```


Gets or sets a value indicating whether this page is a conflict page.

--------------------

The conflict page arises when two users try to update the same content. In this case the changes of first user are written as usual. But changes of another user can't be merged. So just a copy of page is created and marked as conflict.

At this version the conflicts are resolved in favor of the first user's changes. So if document has conflict pages then they will be shown in history but they will be skipped on saving. It is possible to reset this flag to save this pages in history as usual ones.

Detailed sample of manipulating by conflict page can be found in the online documentation.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Gets or sets the creation time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Gets or sets the last modified time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date |  |

### setLevel(byte value) {#setLevel-byte-}
```
public void setLevel(byte value)
```


Gets or sets the level.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte |  |

### setMargin(Margins value) {#setMargin-com.aspose.note.Margins-}
```
public void setMargin(Margins value)
```


Gets or sets the margin.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Margins](../../com.aspose.note/margins) |  |

### setPageContentRevisionSummary(RevisionSummary value) {#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-}
```
public void setPageContentRevisionSummary(RevisionSummary value)
```


Gets or sets the revision summary for the page and it's child nodes.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [RevisionSummary](../../com.aspose.note/revisionsummary) |  |

### setPageLayoutSize(Dimension2D value) {#setPageLayoutSize-java.awt.geom.Dimension2D-}
```
public final void setPageLayoutSize(Dimension2D value)
```


Sets page's layout size displayed in the editor.

--------------------

This value is used by Microsoft OneNote application to display underlying page layout when document is opened. It doesn't affect printing and saving of the document anyway. When Page.SizeType property is set to PageSizeType.SizeByContent this property returns real size of the content.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.awt.geom.Dimension2D |  |

### setSizeType(int value) {#setSizeType-int-}
```
public final void setSizeType(int value)
```


Gets or sets the size type of a page.

--------------------

By default, a page resizes automatically. The default value is [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTitle(Title value) {#setTitle-com.aspose.note.Title-}
```
public void setTitle(Title value)
```


Gets or sets the title.

Value: The  Title .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Title](../../com.aspose.note/title) |  |

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

