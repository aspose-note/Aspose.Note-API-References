---
title: Image
second_title: Aspose.Note for Java API Reference
description: Represents an Image.
type: docs
weight: 33
url: /java/com.aspose.note/image/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public final class Image extends CompositeNode<Loop> implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

Represents an Image.
## Constructors

| Constructor | Description |
| --- | --- |
| [Image(String path)](#Image-java.lang.String-) | Initializes a new instance of the `Image` class. |
| [Image(String fileName, InputStream imageStream)](#Image-java.lang.String-java.io.InputStream-) | Initializes a new instance of the `Image` class. |
| [Image()](#Image--) | Initializes a new instance of the `Image` class. |
## Methods

| Method | Description |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepts the visitor of the node. |
| [getAlignment()](#getAlignment--) | Gets the alignment. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | Gets a body an alternative text for the image. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | Gets a title of alternative text for the image. |
| [getBytes()](#getBytes--) | Gets the image data store. |
| [getFileName()](#getFileName--) | Gets the file name. |
| [getFilePath()](#getFilePath--) | Gets the path to the image file. |
| [getFormat()](#getFormat--) | Gets the image's format. |
| [getHeight()](#getHeight--) | Gets the height. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Gets the horizontal offset. |
| [getHyperlinkUrl()](#getHyperlinkUrl--) | Gets the hyperlink associated with the image. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Gets last modified time. |
| [getOriginalHeight()](#getOriginalHeight--) | Gets the original height. |
| [getOriginalWidth()](#getOriginalWidth--) | Gets the original width. |
| [getTags()](#getTags--) | Gets the list of all tags of an image. |
| [getVerticalOffset()](#getVerticalOffset--) | Gets the vertical offset. |
| [getWidth()](#getWidth--) | Gets the width. |
| [isBackground()](#isBackground--) | Gets whether the image is a background image. |
| [replace(Image newImage)](#replace-com.aspose.note.Image-) | Replaces the current image data with the data from the provided Image object. |
| [setAlignment(int value)](#setAlignment-int-) | Sets the alignment. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | Sets a body an alternative text for the image. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | Sets a title of alternative text for the image. |
| [setBackground(boolean value)](#setBackground-boolean-) | Gets whether the image is a background image. |
| [setHeight(float value)](#setHeight-float-) | Sets the height. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Sets the horizontal offset. |
| [setHyperlinkUrl(String value)](#setHyperlinkUrl-java.lang.String-) | Sets the hyperlink associated with the image. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Sets last modified time. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Sets the vertical offset. |
| [setWidth(float value)](#setWidth-float-) | Sets the width. |
### Image(String path) {#Image-java.lang.String-}
```
public Image(String path)
```


Initializes a new instance of the `Image` class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | A string that contains the path to the file from which to create the `Image`. |

### Image(String fileName, InputStream imageStream) {#Image-java.lang.String-java.io.InputStream-}
```
public Image(String fileName, InputStream imageStream)
```


Initializes a new instance of the `Image` class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | A name of the image. |
| imageStream | java.io.InputStream | A stream which contains the image. |

### Image() {#Image--}
```
public Image()
```


Initializes a new instance of the `Image` class.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepts the visitor of the node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | The object of a class derived from the `DocumentVisitor`. |

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


Gets a body an alternative text for the image.

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


Gets a title of alternative text for the image.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


Gets the image data store.

**Returns:**
byte[]
### getFileName() {#getFileName--}
```
public String getFileName()
```


Gets the file name.

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Gets the path to the image file.

**Returns:**
java.lang.String
### getFormat() {#getFormat--}
```
public final System.Drawing.Imaging.ImageFormat getFormat()
```


Gets the image's format.

**Returns:**
com.aspose.ms.System.Drawing.Imaging.ImageFormat
### getHeight() {#getHeight--}
```
public final float getHeight()
```


Gets the height. This is the real height of the image in the MS OneNote document.

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Gets the horizontal offset.

**Returns:**
float
### getHyperlinkUrl() {#getHyperlinkUrl--}
```
public String getHyperlinkUrl()
```


Gets the hyperlink associated with the image.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Gets last modified time.

**Returns:**
java.util.Date
### getOriginalHeight() {#getOriginalHeight--}
```
public float getOriginalHeight()
```


Gets the original height. This is the original width of the image, before resizing.

**Returns:**
float
### getOriginalWidth() {#getOriginalWidth--}
```
public float getOriginalWidth()
```


Gets the original width. This is the original width of the image, before resizing.

**Returns:**
float
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Gets the list of all tags of an image.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Gets the vertical offset.

**Returns:**
float
### getWidth() {#getWidth--}
```
public final float getWidth()
```


Gets the width. This is the real width of the image in the MS OneNote document.

**Returns:**
float
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


Gets whether the image is a background image.

**Returns:**
boolean
### replace(Image newImage) {#replace-com.aspose.note.Image-}
```
public void replace(Image newImage)
```


Replaces the current image data with the data from the provided Image object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| newImage | [Image](../../com.aspose.note/image) |  |

### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Sets the alignment.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


Sets a body an alternative text for the image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


Sets a title of alternative text for the image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setBackground(boolean value) {#setBackground-boolean-}
```
public final void setBackground(boolean value)
```


Gets whether the image is a background image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHeight(float value) {#setHeight-float-}
```
public final void setHeight(float value)
```


Sets the height. This is the real height of the image in the MS OneNote document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Sets the horizontal offset.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |

### setHyperlinkUrl(String value) {#setHyperlinkUrl-java.lang.String-}
```
public void setHyperlinkUrl(String value)
```


Sets the hyperlink associated with the image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Sets last modified time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Sets the vertical offset.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |

### setWidth(float value) {#setWidth-float-}
```
public final void setWidth(float value)
```


Sets the width. This is the real width of the image in the MS OneNote document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |

