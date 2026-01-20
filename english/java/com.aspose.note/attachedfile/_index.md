---
title: AttachedFile
second_title: Aspose.Note for Java API Reference
description: Represents an attached file.
type: docs
weight: 11
url: /java/com.aspose.note/attachedfile/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public class AttachedFile extends Node implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

Represents an attached file.
## Constructors

| Constructor | Description |
| --- | --- |
| [AttachedFile(String path)](#AttachedFile-java.lang.String-) | Initializes a new instance of the  AttachedFile  class. |
| [AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | Initializes a new instance of the  AttachedFile  class. |
| [AttachedFile(String fileName, InputStream attachedFileStream)](#AttachedFile-java.lang.String-java.io.InputStream-) | Initializes a new instance of the  AttachedFile  class. |
| [AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | Initializes a new instance of the  AttachedFile  class. |
| [AttachedFile()](#AttachedFile--) | Initializes a new instance of the  AttachedFile  class. |
## Methods

| Method | Description |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepts the visitor of the node. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlignment()](#getAlignment--) | Gets the alignment. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | Gets or sets a body an alternative text for the icon of the attached file. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | Gets or sets a title of alternative text for the icon of the attached file. |
| [getBytes()](#getBytes--) | Gets the binary data for an embedded file. |
| [getClass()](#getClass--) |  |
| [getDocument()](#getDocument--) | Gets the document of the node. |
| [getExtension()](#getExtension--) | Gets the extension of an embedded file. |
| [getFileName()](#getFileName--) | Gets the name of the embedded file. |
| [getFilePath()](#getFilePath--) | Gets the path to the original file. |
| [getHeight()](#getHeight--) | Gets the original height of the embedded file icon. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Gets the horizontal offset. |
| [getIcon()](#getIcon--) | Gets the binary data for the icon that is associated with the embedded file. |
| [getIconExtension()](#getIconExtension--) | Gets the extension of the icon. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Gets the last modified time. |
| [getMaxHeight()](#getMaxHeight--) | Gets the maximum height to display the embedded file icon. |
| [getMaxWidth()](#getMaxWidth--) | Gets the maximum width to display the embedded file icon. |
| [getNextSibling()](#getNextSibling--) | Gets the next node at the same node tree level. |
| [getNodeId()](#getNodeId--) | Gets the node's ID. |
| [getNodeType()](#getNodeType--) | Gets the node type. |
| [getParentNode()](#getParentNode--) | Gets the parent node. |
| [getParsingErrorInfo()](#getParsingErrorInfo--) | Gets the data about error that occurred while accessing the file. |
| [getPreviousSibling()](#getPreviousSibling--) | Gets the previous node at the same node tree level. |
| [getTags()](#getTags--) | Gets the list of tags of an attached file. |
| [getText()](#getText--) | Gets the text representation of the embedded file. |
| [getVerticalOffset()](#getVerticalOffset--) | Gets the vertical offset. |
| [getWidth()](#getWidth--) | Gets the original width of the embedded file icon. |
| [hashCode()](#hashCode--) |  |
| [isComposite()](#isComposite--) | Gets a value indicating whether this node is composite. |
| [isPrintout()](#isPrintout--) | Gets a value indicating whether the view of the file is printout. |
| [isSizeSetByUser()](#isSizeSetByUser--) | Gets a value indicating whether the value of the size of the icon was explicitly updated by the user. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignment(int value)](#setAlignment-int-) | Sets the alignment. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | Gets or sets a body an alternative text for the icon of the attached file. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | Gets or sets a title of alternative text for the icon of the attached file. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Sets the horizontal offset. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Sets the last modified time. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | Sets the maximum height to display the embedded file icon. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | Sets the maximum width to display the embedded file icon. |
| [setPrintout(boolean value)](#setPrintout-boolean-) | Sets a value indicating whether the view of the file is printout. |
| [setSizeSetByUser(boolean value)](#setSizeSetByUser-boolean-) | Sets a value indicating whether the value of the size of the icon was explicitly updated by the user. |
| [setText(String value)](#setText-java.lang.String-) | Sets the text representation of the embedded file. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Sets the vertical offset. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AttachedFile(String path) {#AttachedFile-java.lang.String-}
```
public AttachedFile(String path)
```


Initializes a new instance of the  AttachedFile  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | A string that contains the path to the file from which to create the  AttachedFile . |

### AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


Initializes a new instance of the  AttachedFile  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | A string that contains the path to the file from which to create the  AttachedFile . |
| icon | java.io.InputStream | An icon for the attached file. |
| iconFormat | com.aspose.ms.System.Drawing.Imaging.ImageFormat |  |

### AttachedFile(String fileName, InputStream attachedFileStream) {#AttachedFile-java.lang.String-java.io.InputStream-}
```
public AttachedFile(String fileName, InputStream attachedFileStream)
```


Initializes a new instance of the  AttachedFile  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | A name of the attached file. |
| attachedFileStream | java.io.InputStream | A stream which contains the attached file bytes. |

### AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


Initializes a new instance of the  AttachedFile  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | A name of the attached file. |
| attachedFileStream | java.io.InputStream | A stream which contains the attached file bytes. |
| icon | java.io.InputStream | An icon for the attached file. |
| iconFormat | com.aspose.ms.System.Drawing.Imaging.ImageFormat | A format of the attached file icon. |

### AttachedFile() {#AttachedFile--}
```
public AttachedFile()
```


Initializes a new instance of the  AttachedFile  class.

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
### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


Gets the alignment.

**Returns:**
int
### getAlternativeTextDescription() {#getAlternativeTextDescription--}
```
public final String getAlternativeTextDescription()
```


Gets or sets a body an alternative text for the icon of the attached file.

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


Gets or sets a title of alternative text for the icon of the attached file.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


Gets the binary data for an embedded file.

**Returns:**
byte[]
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
### getExtension() {#getExtension--}
```
public String getExtension()
```


Gets the extension of an embedded file.

**Returns:**
java.lang.String
### getFileName() {#getFileName--}
```
public String getFileName()
```


Gets the name of the embedded file.

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Gets the path to the original file.

**Returns:**
java.lang.String
### getHeight() {#getHeight--}
```
public float getHeight()
```


Gets the original height of the embedded file icon.

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Gets the horizontal offset.

**Returns:**
float
### getIcon() {#getIcon--}
```
public byte[] getIcon()
```


Gets the binary data for the icon that is associated with the embedded file.

**Returns:**
byte[]
### getIconExtension() {#getIconExtension--}
```
public String getIconExtension()
```


Gets the extension of the icon.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Gets the last modified time.

**Returns:**
java.util.Date
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


Gets the maximum height to display the embedded file icon.

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Gets the maximum width to display the embedded file icon.

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
### getParsingErrorInfo() {#getParsingErrorInfo--}
```
public final ParsingErrorInfo getParsingErrorInfo()
```


Gets the data about error that occurred while accessing the file.

**Returns:**
[ParsingErrorInfo](../../com.aspose.note.infrastructure/parsingerrorinfo)
### getPreviousSibling() {#getPreviousSibling--}
```
public INode getPreviousSibling()
```


Gets the previous node at the same node tree level.

Value: The previous sibling.

**Returns:**
[INode](../../com.aspose.note/inode)
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Gets the list of tags of an attached file.

**Returns:**
com.aspose.ms.System.Collections.Generic.List<com.aspose.note.ITag>
### getText() {#getText--}
```
public String getText()
```


Gets the text representation of the embedded file. The string MUST NOT contain any characters of the value 10 (line feed) or 13 (carriage return).

**Returns:**
java.lang.String
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Gets the vertical offset.

**Returns:**
float
### getWidth() {#getWidth--}
```
public float getWidth()
```


Gets the original width of the embedded file icon.

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
### isPrintout() {#isPrintout--}
```
public boolean isPrintout()
```


Gets a value indicating whether the view of the file is printout.

**Returns:**
boolean
### isSizeSetByUser() {#isSizeSetByUser--}
```
public boolean isSizeSetByUser()
```


Gets a value indicating whether the value of the size of the icon was explicitly updated by the user.

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




### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Sets the alignment.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | Alignment's value. |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


Gets or sets a body an alternative text for the icon of the attached file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


Gets or sets a title of alternative text for the icon of the attached file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Sets the horizontal offset.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float | Offsets's value. |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Sets the last modified time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | Date's value. |

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


Sets the maximum height to display the embedded file icon.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float | Maximum height's value. |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


Sets the maximum width to display the embedded file icon.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float | Maximum width's value. |

### setPrintout(boolean value) {#setPrintout-boolean-}
```
public void setPrintout(boolean value)
```


Sets a value indicating whether the view of the file is printout.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | New value. |

### setSizeSetByUser(boolean value) {#setSizeSetByUser-boolean-}
```
public void setSizeSetByUser(boolean value)
```


Sets a value indicating whether the value of the size of the icon was explicitly updated by the user.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | New value. |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Sets the text representation of the embedded file. The string MUST NOT contain any characters of the value 10 (line feed) or 13 (carriage return).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | Text's value. |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Sets the vertical offset.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float | Offset's value. |

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

