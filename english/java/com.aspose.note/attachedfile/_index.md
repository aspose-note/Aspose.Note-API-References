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
| [AttachedFile(Document document, String path)](#AttachedFile-com.aspose.note.Document-java.lang.String-) | Initializes a new instance of the  AttachedFile  class. |
| [AttachedFile(Document document, String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-com.aspose.note.Document-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | Initializes a new instance of the  AttachedFile  class. |
| [AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | Initializes a new instance of the [AttachedFile](../../com.aspose.note/attachedfile) class. |
| [AttachedFile(Document document, String fileName, InputStream attachedFileStream)](#AttachedFile-com.aspose.note.Document-java.lang.String-java.io.InputStream-) | Initializes a new instance of the  AttachedFile  class. |
| [AttachedFile(String fileName, InputStream attachedFileStream)](#AttachedFile-java.lang.String-java.io.InputStream-) | Initializes a new instance of the [AttachedFile](../../com.aspose.note/attachedfile) class. |
| [AttachedFile(Document document, String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-com.aspose.note.Document-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | Initializes a new instance of the  AttachedFile  class. |
| [AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | Initializes a new instance of the [AttachedFile](../../com.aspose.note/attachedfile) class. |
| [AttachedFile(Document document)](#AttachedFile-com.aspose.note.Document-) | Initializes a new instance of the  AttachedFile  class. |
| [AttachedFile()](#AttachedFile--) | Initializes a new instance of the [AttachedFile](../../com.aspose.note/attachedfile) class. |
## Methods

| Method | Description |
| --- | --- |
| [getLastModifiedTime()](#getLastModifiedTime--) | Gets the last modified time. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Sets the last modified time. |
| [getMaxWidth()](#getMaxWidth--) | Gets the maximum width to display the embedded file icon. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | Sets the maximum width to display the embedded file icon. |
| [getMaxHeight()](#getMaxHeight--) | Gets the maximum height to display the embedded file icon. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | Sets the maximum height to display the embedded file icon. |
| [isSizeSetByUser()](#isSizeSetByUser--) | Gets a value indicating whether the value of the size of the icon was explicitly updated by the user. |
| [setSizeSetByUser(boolean value)](#setSizeSetByUser-boolean-) | Sets a value indicating whether the value of the size of the icon was explicitly updated by the user. |
| [getText()](#getText--) | Gets the text representation of the embedded file. |
| [setText(String value)](#setText-java.lang.String-) | Sets the text representation of the embedded file. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | Gets or sets a title of alternative text for the icon of the attached file. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | Gets or sets a title of alternative text for the icon of the attached file. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | Gets or sets a body an alternative text for the icon of the attached file. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | Gets or sets a body an alternative text for the icon of the attached file. |
| [getAlignment()](#getAlignment--) | Gets the alignment. |
| [setAlignment(int value)](#setAlignment-int-) | Sets the alignment. |
| [getFileName()](#getFileName--) | Gets the name of the embedded file. |
| [getFilePath()](#getFilePath--) | Gets the path to the original file. |
| [getWidth()](#getWidth--) | Gets the original width of the embedded file icon. |
| [getHeight()](#getHeight--) | Gets the original height of the embedded file icon. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Gets the horizontal offset. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Sets the horizontal offset. |
| [getVerticalOffset()](#getVerticalOffset--) | Gets the vertical offset. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Sets the vertical offset. |
| [getIcon()](#getIcon--) | Gets the binary data for the icon that is associated with the embedded file. |
| [getIconExtension()](#getIconExtension--) | Gets the extension of the icon. |
| [getBytes()](#getBytes--) | Gets the binary data for an embedded file. |
| [getExtension()](#getExtension--) | Gets the extension of an embedded file. |
| [isPrintout()](#isPrintout--) | Gets a value indicating whether the view of the file is printout. |
| [setPrintout(boolean value)](#setPrintout-boolean-) | Sets a value indicating whether the view of the file is printout. |
| [getTags()](#getTags--) | Gets the list of tags of an attached file. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepts the visitor of the node. |
### AttachedFile(Document document, String path) {#AttachedFile-com.aspose.note.Document-java.lang.String-}
```
public AttachedFile(Document document, String path)
```


Initializes a new instance of the  AttachedFile  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | A parent document of the attached file. |
| path | java.lang.String | A string that contains the path to the file from which to create the  AttachedFile . |

### AttachedFile(Document document, String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-com.aspose.note.Document-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(Document document, String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


Initializes a new instance of the  AttachedFile  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | A parent document of the attached file. |
| path | java.lang.String | A string that contains the path to the file from which to create the  AttachedFile . |
| icon | java.io.InputStream | An icon for the attached file. |
| iconFormat | com.aspose.ms.System.Drawing.Imaging.ImageFormat | A format of the attached file icon. |

### AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


Initializes a new instance of the [AttachedFile](../../com.aspose.note/attachedfile) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | A string that contains the path to the file from which to create the [AttachedFile](../../com.aspose.note/attachedfile). |
| icon | java.io.InputStream | An icon for the attached file. |
| iconFormat | com.aspose.ms.System.Drawing.Imaging.ImageFormat | A format of the attached file icon. |

### AttachedFile(Document document, String fileName, InputStream attachedFileStream) {#AttachedFile-com.aspose.note.Document-java.lang.String-java.io.InputStream-}
```
public AttachedFile(Document document, String fileName, InputStream attachedFileStream)
```


Initializes a new instance of the  AttachedFile  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | A parent document of the attached file. |
| fileName | java.lang.String | A name of the attached file. |
| attachedFileStream | java.io.InputStream | A stream which contains the attached file bytes. |

### AttachedFile(String fileName, InputStream attachedFileStream) {#AttachedFile-java.lang.String-java.io.InputStream-}
```
public AttachedFile(String fileName, InputStream attachedFileStream)
```


Initializes a new instance of the [AttachedFile](../../com.aspose.note/attachedfile) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | A name of the attached file. |
| attachedFileStream | java.io.InputStream | A stream which contains the attached file bytes. |

### AttachedFile(Document document, String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-com.aspose.note.Document-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(Document document, String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


Initializes a new instance of the  AttachedFile  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | A parent document of the attached file. |
| fileName | java.lang.String | A name of the attached file. |
| attachedFileStream | java.io.InputStream | A stream which contains the attached file bytes. |
| icon | java.io.InputStream | An icon for the attached file. |
| iconFormat | com.aspose.ms.System.Drawing.Imaging.ImageFormat | A format of the attached file icon. |

### AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


Initializes a new instance of the [AttachedFile](../../com.aspose.note/attachedfile) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | A name of the attached file. |
| attachedFileStream | java.io.InputStream | A stream which contains the attached file bytes. |
| icon | java.io.InputStream | An icon for the attached file. |
| iconFormat | com.aspose.ms.System.Drawing.Imaging.ImageFormat | A format of the attached file icon. |

### AttachedFile(Document document) {#AttachedFile-com.aspose.note.Document-}
```
public AttachedFile(Document document)
```


Initializes a new instance of the  AttachedFile  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | The document of the composite node. |

### AttachedFile() {#AttachedFile--}
```
public AttachedFile()
```


Initializes a new instance of the [AttachedFile](../../com.aspose.note/attachedfile) class.

### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Gets the last modified time.

**Returns:**
java.util.Date
### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Sets the last modified time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | Date's value. |

### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Gets the maximum width to display the embedded file icon.

**Returns:**
float
### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


Sets the maximum width to display the embedded file icon.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float | Maximum width's value. |

### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


Gets the maximum height to display the embedded file icon.

**Returns:**
float
### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


Sets the maximum height to display the embedded file icon.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float | Maximum height's value. |

### isSizeSetByUser() {#isSizeSetByUser--}
```
public boolean isSizeSetByUser()
```


Gets a value indicating whether the value of the size of the icon was explicitly updated by the user.

**Returns:**
boolean
### setSizeSetByUser(boolean value) {#setSizeSetByUser-boolean-}
```
public void setSizeSetByUser(boolean value)
```


Sets a value indicating whether the value of the size of the icon was explicitly updated by the user.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | New value. |

### getText() {#getText--}
```
public String getText()
```


Gets the text representation of the embedded file. The string MUST NOT contain any characters of the value 10 (line feed) or 13 (carriage return).

**Returns:**
java.lang.String
### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Sets the text representation of the embedded file. The string MUST NOT contain any characters of the value 10 (line feed) or 13 (carriage return).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | Text's value. |

### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


Gets or sets a title of alternative text for the icon of the attached file.

**Returns:**
java.lang.String
### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


Gets or sets a title of alternative text for the icon of the attached file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### getAlternativeTextDescription() {#getAlternativeTextDescription--}
```
public final String getAlternativeTextDescription()
```


Gets or sets a body an alternative text for the icon of the attached file.

**Returns:**
java.lang.String
### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


Gets or sets a body an alternative text for the icon of the attached file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


Gets the alignment.

**Returns:**
int
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Sets the alignment.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | Alignment's value. |

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
### getWidth() {#getWidth--}
```
public float getWidth()
```


Gets the original width of the embedded file icon.

**Returns:**
float
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
### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Sets the horizontal offset.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float | Offsets's value. |

### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Gets the vertical offset.

**Returns:**
float
### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Sets the vertical offset.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float | Offset's value. |

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
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


Gets the binary data for an embedded file.

**Returns:**
byte[]
### getExtension() {#getExtension--}
```
public String getExtension()
```


Gets the extension of an embedded file.

**Returns:**
java.lang.String
### isPrintout() {#isPrintout--}
```
public boolean isPrintout()
```


Gets a value indicating whether the view of the file is printout.

**Returns:**
boolean
### setPrintout(boolean value) {#setPrintout-boolean-}
```
public void setPrintout(boolean value)
```


Sets a value indicating whether the view of the file is printout.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | New value. |

### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Gets the list of tags of an attached file.

**Returns:**
com.aspose.ms.System.Collections.Generic.List<com.aspose.note.ITag>
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepts the visitor of the node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | The object of a class derived from the  DocumentVisitor . |

