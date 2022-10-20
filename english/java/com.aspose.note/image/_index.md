---
title: Image
second_title: Aspose.Note for Java API Reference
description: Represents an Image.
type: docs
weight: 25
url: /java/com.aspose.note/image/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public final class Image extends Node implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

Represents an Image.
## Constructors

| Constructor | Description |
| --- | --- |
| [Image(Document document, String path)](#Image-com.aspose.note.Document-java.lang.String-) | Initializes a new instance of the  Image  class. |
| [Image(Document document, String fileName, InputStream imageStream)](#Image-com.aspose.note.Document-java.lang.String-java.io.InputStream-) | Initializes a new instance of the  Image  class. |
| [Image(String fileName, InputStream imageStream)](#Image-java.lang.String-java.io.InputStream-) | Initializes a new instance of the [Image](../../com.aspose.note/image) class. |
| [Image(Document document)](#Image-com.aspose.note.Document-) | Initializes a new instance of the  Image  class. |
| [Image()](#Image--) | Initializes a new instance of the [Image](../../com.aspose.note/image) class. |
## Methods

| Method | Description |
| --- | --- |
| [getLastModifiedTime()](#getLastModifiedTime--) | Gets last modified time. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Sets last modified time. |
| [getWidth()](#getWidth--) | Gets the width. |
| [setWidth(float value)](#setWidth-float-) | Sets the width. |
| [getHeight()](#getHeight--) | Gets the height. |
| [setHeight(float value)](#setHeight-float-) | Sets the height. |
| [isBackground()](#isBackground--) | Gets whether the image is a background image. |
| [setBackground(boolean value)](#setBackground-boolean-) | Gets whether the image is a background image. |
| [getOriginalWidth()](#getOriginalWidth--) | Gets the original width. |
| [getOriginalHeight()](#getOriginalHeight--) | Gets the original height. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Gets the horizontal offset. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Sets the horizontal offset. |
| [getVerticalOffset()](#getVerticalOffset--) | Gets the vertical offset. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Sets the vertical offset. |
| [getFilePath()](#getFilePath--) | Gets the path to the image file. |
| [getFileName()](#getFileName--) | Gets the file name. |
| [getFormat()](#getFormat--) | Gets the image's format. |
| [getBytes()](#getBytes--) | Gets the image data store. |
| [getTags()](#getTags--) | Gets the list of all tags of an image. |
| [getAlignment()](#getAlignment--) | Gets the alignment. |
| [setAlignment(int value)](#setAlignment-int-) | Sets the alignment. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | Gets a title of alternative text for the image. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | Sets a title of alternative text for the image. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | Gets a body an alternative text for the image. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | Sets a body an alternative text for the image. |
| [getHyperlinkUrl()](#getHyperlinkUrl--) | Gets the hyperlink associated with the image. |
| [setHyperlinkUrl(String value)](#setHyperlinkUrl-java.lang.String-) | Sets the hyperlink associated with the image. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepts the visitor of the node. |
### Image(Document document, String path) {#Image-com.aspose.note.Document-java.lang.String-}
```
public Image(Document document, String path)
```


Initializes a new instance of the  Image  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | A parent document of the image. |
| path | java.lang.String | A string that contains the path to the file from which to create the  Image . |

### Image(Document document, String fileName, InputStream imageStream) {#Image-com.aspose.note.Document-java.lang.String-java.io.InputStream-}
```
public Image(Document document, String fileName, InputStream imageStream)
```


Initializes a new instance of the  Image  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | A parent document of the image. |
| fileName | java.lang.String | A name of the image. |
| imageStream | java.io.InputStream | A stream which contains the image. |

### Image(String fileName, InputStream imageStream) {#Image-java.lang.String-java.io.InputStream-}
```
public Image(String fileName, InputStream imageStream)
```


Initializes a new instance of the [Image](../../com.aspose.note/image) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | A name of the image. |
| imageStream | java.io.InputStream | A stream which contains the image. |

### Image(Document document) {#Image-com.aspose.note.Document-}
```
public Image(Document document)
```


Initializes a new instance of the  Image  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | A parent document of the image. |

### Image() {#Image--}
```
public Image()
```


Initializes a new instance of the [Image](../../com.aspose.note/image) class.

### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Gets last modified time.

**Returns:**
java.util.Date
### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Sets last modified time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date |  |

### getWidth() {#getWidth--}
```
public float getWidth()
```


Gets the width. This is the real width of the image in the MS OneNote document.

**Returns:**
float
### setWidth(float value) {#setWidth-float-}
```
public void setWidth(float value)
```


Sets the width. This is the real width of the image in the MS OneNote document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |

### getHeight() {#getHeight--}
```
public float getHeight()
```


Gets the height. This is the real height of the image in the MS OneNote document.

**Returns:**
float
### setHeight(float value) {#setHeight-float-}
```
public void setHeight(float value)
```


Sets the height. This is the real height of the image in the MS OneNote document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |

### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


Gets whether the image is a background image.

**Returns:**
boolean
### setBackground(boolean value) {#setBackground-boolean-}
```
public final void setBackground(boolean value)
```


Gets whether the image is a background image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### getOriginalWidth() {#getOriginalWidth--}
```
public float getOriginalWidth()
```


Gets the original width. This is the original width of the image, before resizing.

**Returns:**
float
### getOriginalHeight() {#getOriginalHeight--}
```
public float getOriginalHeight()
```


Gets the original height. This is the original width of the image, before resizing.

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
| value | float |  |

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
| value | float |  |

### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Gets the path to the image file.

**Returns:**
java.lang.String
### getFileName() {#getFileName--}
```
public String getFileName()
```


Gets the file name.

**Returns:**
java.lang.String
### getFormat() {#getFormat--}
```
public final System.Drawing.Imaging.ImageFormat getFormat()
```


Gets the image's format.

**Returns:**
com.aspose.ms.System.Drawing.Imaging.ImageFormat
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


Gets the image data store.

**Returns:**
byte[]
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Gets the list of all tags of an image.

**Returns:**
com.aspose.ms.System.Collections.Generic.List<com.aspose.note.ITag>
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
| value | int |  |

### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


Gets a title of alternative text for the image.

**Returns:**
java.lang.String
### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


Sets a title of alternative text for the image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### getAlternativeTextDescription() {#getAlternativeTextDescription--}
```
public final String getAlternativeTextDescription()
```


Gets a body an alternative text for the image.

**Returns:**
java.lang.String
### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


Sets a body an alternative text for the image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### getHyperlinkUrl() {#getHyperlinkUrl--}
```
public String getHyperlinkUrl()
```


Gets the hyperlink associated with the image.

**Returns:**
java.lang.String
### setHyperlinkUrl(String value) {#setHyperlinkUrl-java.lang.String-}
```
public void setHyperlinkUrl(String value)
```


Sets the hyperlink associated with the image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepts the visitor of the node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | The object of a class derived from the  DocumentVisitor . |

