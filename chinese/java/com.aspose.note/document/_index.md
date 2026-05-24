---
title: "Document"
second_title: "Aspose.Note for Java API 参考"
description: "表示 Aspose.Note 文档。"
type: docs
weight: 20
url: /zh/java/com.aspose.note/document/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode)
```
public class Document extends CompositeNode<Page> implements INotebookChildNode
```

表示 Aspose.Note 文档。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Document()](#Document--) | 初始化 `Document` 类的新实例。 |
| [Document(String filePath)](#Document-java.lang.String-) | 初始化 `Document` 类的新实例。 |
| [Document(String filePath, LoadOptions loadOptions)](#Document-java.lang.String-com.aspose.note.LoadOptions-) | 初始化 `Document` 类的新实例。 |
| [Document(InputStream inStream)](#Document-java.io.InputStream-) | 初始化 `Document` 类的新实例。 |
| [Document(InputStream inStream, LoadOptions loadOptions)](#Document-java.io.InputStream-com.aspose.note.LoadOptions-) | 初始化 `Document` 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | 接受节点的访问者。 |
| [detectLayoutChanges()](#detectLayoutChanges--) | 检测自上一次 `DetectLayoutChanges` 调用以来对文档布局所做的所有更改。 |
| [getAutomaticLayoutChangesDetectionEnabled()](#getAutomaticLayoutChangesDetectionEnabled--) | 获取指示 Aspose.Note 是否自动执行布局更改检测的值。 |
| [getColor()](#getColor--) | 获取颜色。 |
| [getCreationTime()](#getCreationTime--) | 获取创建时间。 |
| [getDisplayName()](#getDisplayName--) | 获取显示名称。 |
| [getFileFormat()](#getFileFormat--) | 获取文件格式（OneNote 2010，OneNote Online）。 |
| [getGuid()](#getGuid--) | 获取对象的全局唯一标识符。 |
| [getGuidInternal()](#getGuidInternal--) |  |
| [getPageHistory(Page page)](#getPageHistory-com.aspose.note.Page-) | 获取包含文档中每页完整历史的 `PageHistory`（最早的位于索引 0）。 |
| [isEncrypted(InputStream stream, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.Document---) | 检查来自流的文档是否已加密。 |
| [isEncrypted(InputStream stream, LoadOptions options, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---) | 检查来自流的文档是否已加密。 |
| [isEncrypted(InputStream stream, String password, Document[] document)](#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---) | 检查来自流的文档是否已加密。 |
| [isEncrypted(String filePath, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.Document---) | 检查来自文件的文档是否已加密。 |
| [isEncrypted(String filePath, LoadOptions options, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---) | 检查来自文件的文档是否已加密。 |
| [isEncrypted(String filePath, String password, Document[] document)](#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---) | 检查来自文件的文档是否已加密。 |
| [print()](#print--) | 使用默认打印机打印文档。 |
| [print(PrintOptions options)](#print-com.aspose.note.PrintOptions-) | 使用默认打印机打印文档。 |
| [print(String printerName)](#print-java.lang.String-) | 使用默认打印机打印文档。 |
| [print(AttributeSet printSettings)](#print-javax.print.attribute.AttributeSet-) | 使用默认打印机打印文档。 |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | 将 OneNote 文档保存到流中。 |
| [save(OutputStream stream, SaveOptions options)](#save-java.io.OutputStream-com.aspose.note.SaveOptions-) | 使用指定的保存选项将 OneNote 文档保存到流中。 |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | 以指定格式将 OneNote 文档保存到流中。 |
| [save(String fileName)](#save-java.lang.String-) | 将 OneNote 文档保存到文件。 |
| [save(String fileName, SaveOptions options)](#save-java.lang.String-com.aspose.note.SaveOptions-) | 使用指定的保存选项将 OneNote 文档保存到文件。 |
| [save(String fileName, int format)](#save-java.lang.String-int-) | 以指定格式将 OneNote 文档保存到文件。 |
| [setAutomaticLayoutChangesDetectionEnabled(boolean value)](#setAutomaticLayoutChangesDetectionEnabled-boolean-) | 设置一个值，指示 Aspose.Note 是否自动执行布局更改检测。 |
| [setColor(Color value)](#setColor-java.awt.Color-) | 设置颜色。 |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | 设置创建时间。 |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | 设置显示名称。 |
### Document() {#Document--}
```
public Document()
```


初始化 `Document` 类的新实例。创建一个空的 OneNote 文档。

### Document(String filePath) {#Document-java.lang.String-}
```
public Document(String filePath)
```


初始化 `Document` 类的新实例。从文件打开现有的 OneNote 文档。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filePath | java.lang.String | 文件路径。 |

### Document(String filePath, LoadOptions loadOptions) {#Document-java.lang.String-com.aspose.note.LoadOptions-}
```
public Document(String filePath, LoadOptions loadOptions)
```


初始化 `Document` 类的新实例。从文件打开现有的 OneNote 文档。允许指定额外选项，例如加密密码。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filePath | java.lang.String | 文件路径。 |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | 用于加载文档的选项。可以为 null。 |

### Document(InputStream inStream) {#Document-java.io.InputStream-}
```
public Document(InputStream inStream)
```


初始化 `Document` 类的新实例。从流中打开现有的 OneNote 文档。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| inStream | java.io.InputStream | 流。 |

### Document(InputStream inStream, LoadOptions loadOptions) {#Document-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public Document(InputStream inStream, LoadOptions loadOptions)
```


初始化 `Document` 类的新实例。从流中打开现有的 OneNote 文档。允许指定额外选项，例如加密密码。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| inStream | java.io.InputStream | 流。 |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | 用于加载文档的选项。可以为 null。 |

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


接受节点的访问者。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | 从 `DocumentVisitor` 派生的类的对象。 |

### detectLayoutChanges() {#detectLayoutChanges--}
```
public void detectLayoutChanges()
```


检测自上一次 `DetectLayoutChanges` 调用以来对文档布局所做的所有更改。如果 `AutomaticLayoutChangesDetectionEnabled` 设置为 true，则在文档导出开始时自动使用。

### getAutomaticLayoutChangesDetectionEnabled() {#getAutomaticLayoutChangesDetectionEnabled--}
```
public boolean getAutomaticLayoutChangesDetectionEnabled()
```


获取一个值，指示 Aspose.Note 是否自动执行布局更改检测。默认值为 `true`。

**Returns:**
boolean
### getColor() {#getColor--}
```
public Color getColor()
```


获取颜色。

**Returns:**
java.awt.Color
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


获取创建时间。

**Returns:**
java.util.Date
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


获取显示名称。

**Returns:**
java.lang.String
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


获取文件格式（OneNote 2010，OneNote Online）。

**Returns:**
int
### getGuid() {#getGuid--}
```
public UUID getGuid()
```


获取对象的全局唯一标识符。

**Returns:**
java.util.UUID
### getGuidInternal() {#getGuidInternal--}
```
public System.Guid getGuidInternal()
```




**Returns:**
com.aspose.ms.System.Guid
### getPageHistory(Page page) {#getPageHistory-com.aspose.note.Page-}
```
public PageHistory getPageHistory(Page page)
```


获取包含文档中每页完整历史的 `PageHistory`（最早的位于索引 0）。当前页面修订可通过 `PageHistory.current` 访问，并与历史版本集合分开存储。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | 页面的当前修订。 |

**Returns:**
[PageHistory](../../com.aspose.note/pagehistory) - The `PageHistory`.
### isEncrypted(InputStream stream, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, Document[] document)
```


检查来自流的文档是否已加密。要进行检查，需要完整加载该文档。因此此方法可能导致性能损失。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.InputStream | 流。 |
| document | [Document\[\]](../../com.aspose.note/document) | 已加载的文档。 |

**Returns:**
boolean - 如果文档已加密则返回 true，否则返回 false。
### isEncrypted(InputStream stream, LoadOptions options, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, LoadOptions options, Document[] document)
```


检查来自流的文档是否已加密。要进行检查，需要完整加载该文档。因此此方法可能导致性能损失。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.InputStream | 流。 |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | 加载选项。 |
| document | [Document\[\]](../../com.aspose.note/document) | 已加载的文档。 |

**Returns:**
boolean - 如果文档已加密则返回 true，否则返回 false。
### isEncrypted(InputStream stream, String password, Document[] document) {#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, String password, Document[] document)
```


检查来自流的文档是否已加密。要进行检查，需要完整加载该文档。因此此方法可能导致性能损失。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.InputStream | 流。 |
| password | java.lang.String | 用于解密文档的密码。 |
| document | [Document\[\]](../../com.aspose.note/document) | 已加载的文档。 |

**Returns:**
boolean - 如果文档已加密则返回 true，否则返回 false。
### isEncrypted(String filePath, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, Document[] document)
```


检查来自文件的文档是否已加密。要进行检查，需要完整加载该文档。因此此方法可能导致性能损失。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filePath | java.lang.String | 文件路径。 |
| document | [Document\[\]](../../com.aspose.note/document) | 已加载的文档。 |

**Returns:**
boolean - 如果文档已加密则返回 true，否则返回 false。
### isEncrypted(String filePath, LoadOptions options, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, LoadOptions options, Document[] document)
```


检查来自文件的文档是否已加密。要进行检查，需要完整加载该文档。因此此方法可能导致性能损失。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filePath | java.lang.String | 文件路径。 |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | 加载选项。 |
| document | [Document\[\]](../../com.aspose.note/document) | 已加载的文档。 |

**Returns:**
boolean - 如果文档已加密则返回 true，否则返回 false。
### isEncrypted(String filePath, String password, Document[] document) {#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, String password, Document[] document)
```


检查来自文件的文档是否已加密。要进行检查，需要完整加载该文档。因此此方法可能导致性能损失。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filePath | java.lang.String | 文件路径。 |
| password | java.lang.String | 用于解密文档的密码。 |
| document | [Document\[\]](../../com.aspose.note/document) | 已加载的文档。 |

**Returns:**
boolean - 如果文档已加密则返回 true，否则返回 false。
### print() {#print--}
```
public void print()
```


使用默认打印机打印文档。

### print(PrintOptions options) {#print-com.aspose.note.PrintOptions-}
```
public void print(PrintOptions options)
```


使用默认打印机打印文档。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| options | [PrintOptions](../../com.aspose.note/printoptions) | 用于打印文档的选项。可以为 null。 |

### print(String printerName) {#print-java.lang.String-}
```
public void print(String printerName)
```


使用默认打印机打印文档。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| printerName | java.lang.String |  |

### print(AttributeSet printSettings) {#print-javax.print.attribute.AttributeSet-}
```
public void print(AttributeSet printSettings)
```


使用默认打印机打印文档。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| printSettings | javax.print.attribute.AttributeSet |  |

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


将 OneNote 文档保存到流中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.OutputStream | 该 System.iO.stream 用于保存文档。 |

### save(OutputStream stream, SaveOptions options) {#save-java.io.OutputStream-com.aspose.note.SaveOptions-}
```
public void save(OutputStream stream, SaveOptions options)
```


使用指定的保存选项将 OneNote 文档保存到流中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.OutputStream | 该 System.iO.stream 用于保存文档。 |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | 指定文档在流中保存的选项。 |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


以指定格式将 OneNote 文档保存到流中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.OutputStream | 该 System.iO.stream 用于保存文档。 |
| format | int | 保存文档的格式。 |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


将 OneNote 文档保存到文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文件名 | java.lang.String | 文件的完整名称。如果具有指定完整名称的文件已存在，则会覆盖现有文件。 |

### save(String fileName, SaveOptions options) {#save-java.lang.String-com.aspose.note.SaveOptions-}
```
public void save(String fileName, SaveOptions options)
```


使用指定的保存选项将 OneNote 文档保存到文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文件名 | java.lang.String | 文件的完整名称。如果具有指定完整名称的文件已存在，则会覆盖现有文件。 |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | 指定文档在文件中保存的选项。 |

### save(String fileName, int format) {#save-java.lang.String-int-}
```
public void save(String fileName, int format)
```


以指定格式将 OneNote 文档保存到文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文件名 | java.lang.String | 文件的完整名称。如果具有指定完整名称的文件已存在，则会覆盖现有文件。 |
| format | int | 保存文档的格式。 |

### setAutomaticLayoutChangesDetectionEnabled(boolean value) {#setAutomaticLayoutChangesDetectionEnabled-boolean-}
```
public void setAutomaticLayoutChangesDetectionEnabled(boolean value)
```


设置一个值，指示 Aspose.Note 是否自动执行布局更改检测。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 新值。可以为 null。 |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


设置颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.awt.Color | 颜色的值。 |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


设置创建时间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | DateTime 的值。 |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


设置显示名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | DateTime 的值。 |

