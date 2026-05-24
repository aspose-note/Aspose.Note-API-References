---
title: "AttachedFile"
second_title: "Aspose.Note for Java API 参考"
description: "表示一个附件文件。"
type: docs
weight: 11
url: /zh/java/com.aspose.note/attachedfile/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public class AttachedFile extends Node implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

表示一个附件文件。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [AttachedFile(String path)](#AttachedFile-java.lang.String-) | 初始化 `AttachedFile` 类的新实例。 |
| [AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | 初始化 `AttachedFile` 类的新实例。 |
| [AttachedFile(String fileName, InputStream attachedFileStream)](#AttachedFile-java.lang.String-java.io.InputStream-) | 初始化 `AttachedFile` 类的新实例。 |
| [AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | 初始化 `AttachedFile` 类的新实例。 |
| [AttachedFile()](#AttachedFile--) | 初始化 `AttachedFile` 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | 接受节点的访问者。 |
| [getAlignment()](#getAlignment--) | 获取对齐方式。 |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | 获取或设置附件文件图标的正文替代文本。 |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | 获取或设置附件文件图标的标题替代文本。 |
| [getBytes()](#getBytes--) | 获取嵌入文件的二进制数据。 |
| [getExtension()](#getExtension--) | 获取嵌入文件的扩展名。 |
| [getFileName()](#getFileName--) | 获取嵌入文件的名称。 |
| [getFilePath()](#getFilePath--) | 获取原始文件的路径。 |
| [getHeight()](#getHeight--) | 获取嵌入文件图标的原始高度。 |
| [getHorizontalOffset()](#getHorizontalOffset--) | 获取水平偏移。 |
| [getIcon()](#getIcon--) | 获取与嵌入文件关联的图标的二进制数据。 |
| [getIconExtension()](#getIconExtension--) | 获取图标的扩展名。 |
| [getLastModifiedTime()](#getLastModifiedTime--) | 获取最后修改时间。 |
| [getMaxHeight()](#getMaxHeight--) | 获取用于显示嵌入文件图标的最大高度。 |
| [getMaxWidth()](#getMaxWidth--) | 获取用于显示嵌入文件图标的最大宽度。 |
| [getParsingErrorInfo()](#getParsingErrorInfo--) | 获取访问文件时发生的错误数据。 |
| [getTags()](#getTags--) | 获取附件文件的标签列表。 |
| [getText()](#getText--) | 获取嵌入文件的文本表示。 |
| [getVerticalOffset()](#getVerticalOffset--) | 获取垂直偏移量。 |
| [getWidth()](#getWidth--) | 获取嵌入文件图标的原始宽度。 |
| [isPrintout()](#isPrintout--) | 获取一个值，指示文件的视图是否为打印输出。 |
| [isSizeSetByUser()](#isSizeSetByUser--) | 获取一个值，指示图标大小的值是否已被用户显式更新。 |
| [setAlignment(int value)](#setAlignment-int-) | 设置对齐方式。 |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | 获取或设置附件文件图标的正文替代文本。 |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | 获取或设置附件文件图标的标题替代文本。 |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | 设置水平偏移量。 |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 设置最后修改时间。 |
| [setMaxHeight(float value)](#setMaxHeight-float-) | 设置用于显示嵌入文件图标的最大高度。 |
| [setMaxWidth(float value)](#setMaxWidth-float-) | 设置用于显示嵌入文件图标的最大宽度。 |
| [setPrintout(boolean value)](#setPrintout-boolean-) | 设置一个值，指示文件的视图是否为打印输出。 |
| [setSizeSetByUser(boolean value)](#setSizeSetByUser-boolean-) | 设置一个值，指示图标大小的值是否已被用户显式更新。 |
| [setText(String value)](#setText-java.lang.String-) | 设置嵌入文件的文本表示。 |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | 设置垂直偏移量。 |
### AttachedFile(String path) {#AttachedFile-java.lang.String-}
```
public AttachedFile(String path)
```


初始化 `AttachedFile` 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | java.lang.String | 一个字符串，包含用于创建 `AttachedFile` 的文件路径。 |

### AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


初始化 `AttachedFile` 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | java.lang.String | 一个字符串，包含用于创建 `AttachedFile` 的文件路径。 |
| 图标 | java.io.InputStream | 附件文件的图标。 |
| 图标格式 | com.aspose.ms.System.Drawing.Imaging.ImageFormat |  |

### AttachedFile(String fileName, InputStream attachedFileStream) {#AttachedFile-java.lang.String-java.io.InputStream-}
```
public AttachedFile(String fileName, InputStream attachedFileStream)
```


初始化 `AttachedFile` 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文件名 | java.lang.String | 附件文件的名称。 |
| attachedFileStream | java.io.InputStream | 包含附件文件字节的流。 |

### AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


初始化 `AttachedFile` 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文件名 | java.lang.String | 附件文件的名称。 |
| attachedFileStream | java.io.InputStream | 包含附件文件字节的流。 |
| 图标 | java.io.InputStream | 附件文件的图标。 |
| 图标格式 | com.aspose.ms.System.Drawing.Imaging.ImageFormat | 附件文件图标的格式。 |

### AttachedFile() {#AttachedFile--}
```
public AttachedFile()
```


初始化 `AttachedFile` 类的新实例。

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


获取或设置附件文件图标的正文替代文本。

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


获取或设置附件文件图标的标题替代文本。

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


获取嵌入文件的二进制数据。

**Returns:**
byte[]
### getExtension() {#getExtension--}
```
public String getExtension()
```


获取嵌入文件的扩展名。

**Returns:**
java.lang.String
### getFileName() {#getFileName--}
```
public String getFileName()
```


获取嵌入文件的名称。

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


获取原始文件的路径。

**Returns:**
java.lang.String
### getHeight() {#getHeight--}
```
public float getHeight()
```


获取嵌入文件图标的原始高度。

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


获取水平偏移。

**Returns:**
float
### getIcon() {#getIcon--}
```
public byte[] getIcon()
```


获取与嵌入文件关联的图标的二进制数据。

**Returns:**
byte[]
### getIconExtension() {#getIconExtension--}
```
public String getIconExtension()
```


获取图标的扩展名。

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


获取最后修改时间。

**Returns:**
java.util.Date
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


获取用于显示嵌入文件图标的最大高度。

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


获取用于显示嵌入文件图标的最大宽度。

**Returns:**
float
### getParsingErrorInfo() {#getParsingErrorInfo--}
```
public final ParsingErrorInfo getParsingErrorInfo()
```


获取访问文件时发生的错误数据。

**Returns:**
[ParsingErrorInfo](../../com.aspose.note.infrastructure/parsingerrorinfo)
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


获取附件文件的标签列表。

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public String getText()
```


获取嵌入文件的文本表示。字符串不得包含值为 10（换行）或 13（回车）的任何字符。

**Returns:**
java.lang.String
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


获取垂直偏移量。

**Returns:**
float
### getWidth() {#getWidth--}
```
public float getWidth()
```


获取嵌入文件图标的原始宽度。

**Returns:**
float
### isPrintout() {#isPrintout--}
```
public boolean isPrintout()
```


获取一个值，指示文件的视图是否为打印输出。

**Returns:**
boolean
### isSizeSetByUser() {#isSizeSetByUser--}
```
public boolean isSizeSetByUser()
```


获取一个值，指示图标大小的值是否已被用户显式更新。

**Returns:**
boolean
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


设置对齐方式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | Alignment 的值。 |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


获取或设置附件文件图标的正文替代文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


获取或设置附件文件图标的标题替代文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


设置水平偏移量。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | float | Offsets 的值。 |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


设置最后修改时间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | Date 的值。 |

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


设置用于显示嵌入文件图标的最大高度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | float | Maximum height 的值。 |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


设置用于显示嵌入文件图标的最大宽度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | float | Maximum width 的值。 |

### setPrintout(boolean value) {#setPrintout-boolean-}
```
public void setPrintout(boolean value)
```


设置一个值，指示文件的视图是否为打印输出。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 新值。 |

### setSizeSetByUser(boolean value) {#setSizeSetByUser-boolean-}
```
public void setSizeSetByUser(boolean value)
```


设置一个值，指示图标大小的值是否已被用户显式更新。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 新值。 |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


设置嵌入文件的文本表示。字符串不得包含值为 10（换行）或 13（回车）的任何字符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | Text 的值。 |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


设置垂直偏移量。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | float | Offset 的值。 |

