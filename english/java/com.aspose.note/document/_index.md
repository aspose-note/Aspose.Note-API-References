---
title: Document
second_title: Aspose.Note for Java API Reference
description: Represents an Aspose.Note document.
type: docs
weight: 20
url: /java/com.aspose.note/document/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode)
```
public class Document extends CompositeNode<Page> implements INotebookChildNode
```

Represents an Aspose.Note document.
## Constructors

| Constructor | Description |
| --- | --- |
| [Document()](#Document--) | Initializes a new instance of the  Document  class. |
| [Document(String filePath)](#Document-java.lang.String-) | Initializes a new instance of the  Document  class. |
| [Document(String filePath, LoadOptions loadOptions)](#Document-java.lang.String-com.aspose.note.LoadOptions-) | Initializes a new instance of the  Document  class. |
| [Document(InputStream inStream)](#Document-java.io.InputStream-) | Initializes a new instance of the  Document  class. |
| [Document(InputStream inStream, LoadOptions loadOptions)](#Document-java.io.InputStream-com.aspose.note.LoadOptions-) | Initializes a new instance of the  Document  class. |
## Methods

| Method | Description |
| --- | --- |
| [<T1>appendChildFirst(T1 newChild)](#-T1-appendChildFirst-T1-) | Adds the node to the front of the list of child nodes for this node. |
| [<T1>appendChildLast(T1 newChild)](#-T1-appendChildLast-T1-) | Adds the node to the end of the list of child nodes for this node. |
| [<T1>getChildNodes(Class<T1> typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Get all child nodes by the node type. |
| [<T1>insertChild(int i, T1 newChild)](#-T1-insertChild-int-T1-) | Inserts the node to the specified position in the list of child nodes for this node. |
| [<T1>removeChild(T1 oldChild)](#-T1-removeChild-T1-) | Removes the child node. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepts the visitor of the node. |
| [detectLayoutChanges()](#detectLayoutChanges--) | Detects all changes made to the document layout since the previous  DetectLayoutChanges  call. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutomaticLayoutChangesDetectionEnabled()](#getAutomaticLayoutChangesDetectionEnabled--) | Gets a value indicating whether Aspose.Note performs detection of layout changes automatically. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Gets the color. |
| [getCreationTime()](#getCreationTime--) | Gets the creation time. |
| [getDisplayName()](#getDisplayName--) | Gets the display name. |
| [getDocument()](#getDocument--) | Gets the document of the node. |
| [getFileFormat()](#getFileFormat--) | Gets file format (OneNote 2010, OneNote Online). |
| [getFirstChild()](#getFirstChild--) | Gets the first child node of this node. |
| [getGuid()](#getGuid--) | Gets the object's globally unique id. |
| [getGuidInternal()](#getGuidInternal--) |  |
| [getLastChild()](#getLastChild--) | Gets the last child node of this node. |
| [getNextSibling()](#getNextSibling--) | Gets the next node at the same node tree level. |
| [getNodeId()](#getNodeId--) | Gets the node's ID. |
| [getNodeType()](#getNodeType--) | Gets the node type. |
| [getPageHistory(Page page)](#getPageHistory-com.aspose.note.Page-) | Gets the  PageHistory  which contains full history for each page presented in a document (the earliest at index 0). |
| [getParentNode()](#getParentNode--) | Gets the parent node. |
| [getPreviousSibling()](#getPreviousSibling--) | Gets the previous node at the same node tree level. |
| [hashCode()](#hashCode--) |  |
| [insertChildrenRange(int i, T[] newChildren)](#insertChildrenRange-int-T...-) | Inserts the node's sequence starting from specified position in the list of child nodes for this node. |
| [insertChildrenRange(int i, Iterable<T> newChildren)](#insertChildrenRange-int-java.lang.Iterable-T--) | Inserts the node's sequence starting from specified position in the list of child nodes for this node. |
| [isComposite()](#isComposite--) | Checks whether the node is composite. |
| [isEncrypted(InputStream stream, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.Document---) | Checks whether a document from a stream is encrypted. |
| [isEncrypted(InputStream stream, LoadOptions options, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---) | Checks whether a document from a stream is encrypted. |
| [isEncrypted(InputStream stream, String password, Document[] document)](#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---) | Checks whether a document from a stream is encrypted. |
| [isEncrypted(String filePath, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.Document---) | Checks whether a document from a file is encrypted. |
| [isEncrypted(String filePath, LoadOptions options, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---) | Checks whether a document from a file is encrypted. |
| [isEncrypted(String filePath, String password, Document[] document)](#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---) | Checks whether a document from a file is encrypted. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through child nodes of the  CompositeNode\{T\} . |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [print()](#print--) | Prints the document using the default printer. |
| [print(PrintOptions options)](#print-com.aspose.note.PrintOptions-) | Prints the document using the default printer. |
| [print(String printerName)](#print-java.lang.String-) | Prints the document using the default printer. |
| [print(AttributeSet printSettings)](#print-javax.print.attribute.AttributeSet-) | Prints the document using the default printer. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Saves the OneNote document to a stream. |
| [save(OutputStream stream, SaveOptions options)](#save-java.io.OutputStream-com.aspose.note.SaveOptions-) | Saves the OneNote document to a stream using the specified save options. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Saves the OneNote document to a stream in the specified format. |
| [save(String fileName)](#save-java.lang.String-) | Saves the OneNote document to a file. |
| [save(String fileName, SaveOptions options)](#save-java.lang.String-com.aspose.note.SaveOptions-) | Saves the OneNote document to a file using the specified save options. |
| [save(String fileName, int format)](#save-java.lang.String-int-) | Saves the OneNote document to a file in the specified format. |
| [setAutomaticLayoutChangesDetectionEnabled(boolean value)](#setAutomaticLayoutChangesDetectionEnabled-boolean-) | Sets a value indicating whether Aspose.Note performs detection of layout changes automatically. |
| [setColor(Color value)](#setColor-java.awt.Color-) | Sets the color. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Sets the creation time. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Sets the display name. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Document() {#Document--}
```
public Document()
```


Initializes a new instance of the  Document  class. Creates a blank OneNote document.

### Document(String filePath) {#Document-java.lang.String-}
```
public Document(String filePath)
```


Initializes a new instance of the  Document  class. Opens an existing OneNote document from a file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file path. |

### Document(String filePath, LoadOptions loadOptions) {#Document-java.lang.String-com.aspose.note.LoadOptions-}
```
public Document(String filePath, LoadOptions loadOptions)
```


Initializes a new instance of the  Document  class. Opens an existing OneNote document from a file. Allows to specify additional options such as an encryption password.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file path. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Options used to load a document. Can be null. |

### Document(InputStream inStream) {#Document-java.io.InputStream-}
```
public Document(InputStream inStream)
```


Initializes a new instance of the  Document  class. Opens an existing OneNote document from a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| inStream | java.io.InputStream | The stream. |

### Document(InputStream inStream, LoadOptions loadOptions) {#Document-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public Document(InputStream inStream, LoadOptions loadOptions)
```


Initializes a new instance of the  Document  class. Opens an existing OneNote document from a stream. Allows to specify additional options such as an encryption password.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| inStream | java.io.InputStream | The stream. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Options used to load a document. Can be null. |

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

### detectLayoutChanges() {#detectLayoutChanges--}
```
public void detectLayoutChanges()
```


Detects all changes made to the document layout since the previous  DetectLayoutChanges  call. In case  AutomaticLayoutChangesDetectionEnabled  set to true, used automatically in the beginning of document export.

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
### getAutomaticLayoutChangesDetectionEnabled() {#getAutomaticLayoutChangesDetectionEnabled--}
```
public boolean getAutomaticLayoutChangesDetectionEnabled()
```


Gets a value indicating whether Aspose.Note performs detection of layout changes automatically. Default value is  true .

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColor() {#getColor--}
```
public Color getColor()
```


Gets the color.

**Returns:**
java.awt.Color
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Gets the creation time.

**Returns:**
java.util.Date
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Gets the display name.

**Returns:**
java.lang.String
### getDocument() {#getDocument--}
```
public Document getDocument()
```


Gets the document of the node.

Value: The document.

**Returns:**
[Document](../../com.aspose.note/document)
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


Gets file format (OneNote 2010, OneNote Online).

**Returns:**
int
### getFirstChild() {#getFirstChild--}
```
public T getFirstChild()
```


Gets the first child node of this node.

**Returns:**
T
### getGuid() {#getGuid--}
```
public UUID getGuid()
```


Gets the object's globally unique id.

**Returns:**
java.util.UUID
### getGuidInternal() {#getGuidInternal--}
```
public System.Guid getGuidInternal()
```




**Returns:**
com.aspose.ms.System.Guid
### getLastChild() {#getLastChild--}
```
public T getLastChild()
```


Gets the last child node of this node.

**Returns:**
T
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
### getPageHistory(Page page) {#getPageHistory-com.aspose.note.Page-}
```
public PageHistory getPageHistory(Page page)
```


Gets the  PageHistory  which contains full history for each page presented in a document (the earliest at index 0). The current page revision can be accessed as  PageHistory.current  and contained separately from collection of historical versions.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | The current revision of a page. |

**Returns:**
[PageHistory](../../com.aspose.note/pagehistory) - The  PageHistory .
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
### isEncrypted(InputStream stream, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, Document[] document)
```


Checks whether a document from a stream is encrypted. To check it we need to completely load this document. So this method can lead to performance penalty.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The stream. |
| document | [Document\[\]](../../com.aspose.note/document) | The loaded document. |

**Returns:**
boolean - Returns true if the document is encrypted otherwise false.
### isEncrypted(InputStream stream, LoadOptions options, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, LoadOptions options, Document[] document)
```


Checks whether a document from a stream is encrypted. To check it we need to completely load this document. So this method can lead to performance penalty.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The stream. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | The load options. |
| document | [Document\[\]](../../com.aspose.note/document) | The loaded document. |

**Returns:**
boolean - Returns true if the document is encrypted otherwise false.
### isEncrypted(InputStream stream, String password, Document[] document) {#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, String password, Document[] document)
```


Checks whether a document from a stream is encrypted. To check it we need to completely load this document. So this method can lead to performance penalty.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The stream. |
| password | java.lang.String | The password to decrypt a document. |
| document | [Document\[\]](../../com.aspose.note/document) | The loaded document. |

**Returns:**
boolean - Returns true if the document is encrypted otherwise false.
### isEncrypted(String filePath, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, Document[] document)
```


Checks whether a document from a file is encrypted. To check it we need to completely load this document. So this method can lead to performance penalty.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file path. |
| document | [Document\[\]](../../com.aspose.note/document) | The loaded document. |

**Returns:**
boolean - Returns true if the document is encrypted otherwise false.
### isEncrypted(String filePath, LoadOptions options, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, LoadOptions options, Document[] document)
```


Checks whether a document from a file is encrypted. To check it we need to completely load this document. So this method can lead to performance penalty.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file path. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | The load options. |
| document | [Document\[\]](../../com.aspose.note/document) | The loaded document. |

**Returns:**
boolean - Returns true if the document is encrypted otherwise false.
### isEncrypted(String filePath, String password, Document[] document) {#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, String password, Document[] document)
```


Checks whether a document from a file is encrypted. To check it we need to completely load this document. So this method can lead to performance penalty.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file path. |
| password | java.lang.String | The password to decrypt a document. |
| document | [Document\[\]](../../com.aspose.note/document) | The loaded document. |

**Returns:**
boolean - Returns true if the document is encrypted otherwise false.
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




### print() {#print--}
```
public void print()
```


Prints the document using the default printer.

### print(PrintOptions options) {#print-com.aspose.note.PrintOptions-}
```
public void print(PrintOptions options)
```


Prints the document using the default printer.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [PrintOptions](../../com.aspose.note/printoptions) | Options used to print a document. Can be null. |

### print(String printerName) {#print-java.lang.String-}
```
public void print(String printerName)
```


Prints the document using the default printer.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String |  |

### print(AttributeSet printSettings) {#print-javax.print.attribute.AttributeSet-}
```
public void print(AttributeSet printSettings)
```


Prints the document using the default printer.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printSettings | javax.print.attribute.AttributeSet |  |

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Saves the OneNote document to a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The System.iO.stream where the document will be saved. |

### save(OutputStream stream, SaveOptions options) {#save-java.io.OutputStream-com.aspose.note.SaveOptions-}
```
public void save(OutputStream stream, SaveOptions options)
```


Saves the OneNote document to a stream using the specified save options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The System.iO.stream where the document will be saved. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | Specifies the options how the document is saved in stream. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


Saves the OneNote document to a stream in the specified format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The System.iO.stream where the document will be saved. |
| format | int | The format in which to save the document. |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


Saves the OneNote document to a file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The full name for the file. If a file with the specified full name already exists, the existing file is overwritten. |

### save(String fileName, SaveOptions options) {#save-java.lang.String-com.aspose.note.SaveOptions-}
```
public void save(String fileName, SaveOptions options)
```


Saves the OneNote document to a file using the specified save options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The full name for the file. If a file with the specified full name already exists, the existing file is overwritten. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | Specifies the options how the document is saved in file. |

### save(String fileName, int format) {#save-java.lang.String-int-}
```
public void save(String fileName, int format)
```


Saves the OneNote document to a file in the specified format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The full name for the file. If a file with the specified full name already exists, the existing file is overwritten. |
| format | int | The format in which to save the document. |

### setAutomaticLayoutChangesDetectionEnabled(boolean value) {#setAutomaticLayoutChangesDetectionEnabled-boolean-}
```
public void setAutomaticLayoutChangesDetectionEnabled(boolean value)
```


Sets a value indicating whether Aspose.Note performs detection of layout changes automatically.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | New value. Can be null. |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


Sets the color.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.awt.Color | Color's value. |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Sets the creation time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | DateTime's value. |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Sets the display name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | DateTime's value. |

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

