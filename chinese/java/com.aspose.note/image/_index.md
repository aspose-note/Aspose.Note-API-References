---
title: "图像"
second_title: "Aspose.Note for Java API 参考"
description: "表示图像。"
type: docs
weight: 33
url: /zh/java/com.aspose.note/image/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public final class Image extends CompositeNode<Loop> implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

表示图像。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Image(String path)](#Image-java.lang.String-) | 初始化 `Image` 类的新实例。 |
| [Image(String fileName, InputStream imageStream)](#Image-java.lang.String-java.io.InputStream-) | 初始化 `Image` 类的新实例。 |
| [Image()](#Image--) | 初始化 `Image` 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | 接受节点的访问者。 |
| [getAlignment()](#getAlignment--) | 获取对齐方式。 |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | 获取图像的主体替代文本。 |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | 获取图像的替代文本标题。 |
| [getBytes()](#getBytes--) | 获取图像数据存储。 |
| [getFileName()](#getFileName--) | 获取文件名。 |
| [getFilePath()](#getFilePath--) | 获取图像文件的路径。 |
| [getFormat()](#getFormat--) | 获取图像的格式。 |
| [getHeight()](#getHeight--) | 获取高度。 |
| [getHorizontalOffset()](#getHorizontalOffset--) | 获取水平偏移。 |
| [getHyperlinkUrl()](#getHyperlinkUrl--) | 获取与图像关联的超链接。 |
| [getLastModifiedTime()](#getLastModifiedTime--) | 获取最后修改时间。 |
| [getOriginalHeight()](#getOriginalHeight--) | 获取原始高度。 |
| [getOriginalWidth()](#getOriginalWidth--) | 获取原始宽度。 |
| [getTags()](#getTags--) | 获取图像的所有标签列表。 |
| [getVerticalOffset()](#getVerticalOffset--) | 获取垂直偏移量。 |
| [getWidth()](#getWidth--) | 获取宽度。 |
| [isBackground()](#isBackground--) | 获取图像是否为背景图像。 |
| [replace(Image newImage)](#replace-com.aspose.note.Image-) | 用提供的 Image 对象中的数据替换当前图像数据。 |
| [setAlignment(int value)](#setAlignment-int-) | 设置对齐方式。 |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | 设置图像的主体替代文本。 |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | 设置图像的替代文本标题。 |
| [setBackground(boolean value)](#setBackground-boolean-) | 获取图像是否为背景图像。 |
| [setHeight(float value)](#setHeight-float-) | 设置高度。 |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | 设置水平偏移量。 |
| [setHyperlinkUrl(String value)](#setHyperlinkUrl-java.lang.String-) | 设置与图像关联的超链接。 |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 设置最后修改时间。 |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | 设置垂直偏移量。 |
| [setWidth(float value)](#setWidth-float-) | 设置宽度。 |
### Image(String path) {#Image-java.lang.String-}
```
public Image(String path)
```


初始化 `Image` 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | java.lang.String | 一个包含用于创建 `Image` 的文件路径的字符串。 |

### Image(String fileName, InputStream imageStream) {#Image-java.lang.String-java.io.InputStream-}
```
public Image(String fileName, InputStream imageStream)
```


初始化 `Image` 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文件名 | java.lang.String | 图像的名称。 |
| imageStream | java.io.InputStream | 包含图像的流。 |

### Image() {#Image--}
```
public Image()
```


初始化 `Image` 类的新实例。

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


接受节点的访问者。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | 从 `DocumentVisitor` 派生的类的对象。 |

### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


获取对齐方式。

**Returns:**
int
### getAlternativeTextDescription() {#getAlternativeTextDescription--}
```
public final String getAlternativeTextDescription()
```


获取图像的主体替代文本。

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


获取图像的替代文本标题。

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


获取图像数据存储。

**Returns:**
byte[]
### getFileName() {#getFileName--}
```
public String getFileName()
```


获取文件名。

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


获取图像文件的路径。

**Returns:**
java.lang.String
### getFormat() {#getFormat--}
```
public final System.Drawing.Imaging.ImageFormat getFormat()
```


获取图像的格式。

**Returns:**
com.aspose.ms.System.Drawing.Imaging.ImageFormat
### getHeight() {#getHeight--}
```
public final float getHeight()
```


获取高度。这是 MS OneNote 文档中图像的实际高度。

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


获取水平偏移。

**Returns:**
float
### getHyperlinkUrl() {#getHyperlinkUrl--}
```
public String getHyperlinkUrl()
```


获取与图像关联的超链接。

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


获取最后修改时间。

**Returns:**
java.util.Date
### getOriginalHeight() {#getOriginalHeight--}
```
public float getOriginalHeight()
```


获取原始高度。这是图像在调整大小之前的原始宽度。

**Returns:**
float
### getOriginalWidth() {#getOriginalWidth--}
```
public float getOriginalWidth()
```


获取原始宽度。这是图像在调整大小之前的原始宽度。

**Returns:**
float
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


获取图像的所有标签列表。

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


获取垂直偏移量。

**Returns:**
float
### getWidth() {#getWidth--}
```
public final float getWidth()
```


获取宽度。这是 MS OneNote 文档中图像的实际宽度。

**Returns:**
float
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


获取图像是否为背景图像。

**Returns:**
boolean
### replace(Image newImage) {#replace-com.aspose.note.Image-}
```
public void replace(Image newImage)
```


用提供的 Image 对象中的数据替换当前图像数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| newImage | [Image](../../com.aspose.note/image) |  |

### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


设置对齐方式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


设置图像的主体替代文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


设置图像的替代文本标题。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setBackground(boolean value) {#setBackground-boolean-}
```
public final void setBackground(boolean value)
```


获取图像是否为背景图像。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHeight(float value) {#setHeight-float-}
```
public final void setHeight(float value)
```


设置高度。这是 MS OneNote 文档中图像的实际高度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | float |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


设置水平偏移量。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | float |  |

### setHyperlinkUrl(String value) {#setHyperlinkUrl-java.lang.String-}
```
public void setHyperlinkUrl(String value)
```


设置与图像关联的超链接。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


设置最后修改时间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


设置垂直偏移量。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | float |  |

### setWidth(float value) {#setWidth-float-}
```
public final void setWidth(float value)
```


设置宽度。这是 MS OneNote 文档中图像的实际宽度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | float |  |

