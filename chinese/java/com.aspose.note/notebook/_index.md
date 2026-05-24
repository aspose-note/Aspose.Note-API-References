---
title: "笔记本"
second_title: "Aspose.Note for Java API 参考"
description: "表示 Aspose.Note 笔记本。"
type: docs
weight: 56
url: /zh/java/com.aspose.note/notebook/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class Notebook implements INotebookChildNode, System.Collections.Generic.IGenericEnumerable<INotebookChildNode>
```

表示 Aspose.Note 笔记本。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Notebook()](#Notebook--) | 初始化 `Notebook` 类的新实例。 |
| [Notebook(String filePath)](#Notebook-java.lang.String-) | 初始化 `Notebook` 类的新实例。 |
| [Notebook(String filePath, NotebookLoadOptions loadOptions)](#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | 初始化 `Notebook` 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | 按节点类型获取所有子节点。 |
| [appendChild(INotebookChildNode newChild)](#appendChild-com.aspose.note.INotebookChildNode-) | 将节点添加到列表末尾。 |
| [getColor()](#getColor--) | 获取或设置颜色。 |
| [getCount()](#getCount--) | 获取 `Notebook` 中包含的元素数量。 |
| [getDisplayName()](#getDisplayName--) | 获取或设置显示名称。 |
| [getFileFormat()](#getFileFormat--) | 获取文件格式（OneNote 2010，OneNote Online）。 |
| [getGuid()](#getGuid--) | 获取对象的全局唯一标识符。 |
| [getGuidInternal()](#getGuidInternal--) |  |
| [get_Item(int index)](#get-Item-int-) | 按给定索引获取笔记本子节点。 |
| [isHistoryEnabled()](#isHistoryEnabled--) | 获取或设置一个值，指示是否启用历史记录。 |
| [iterator()](#iterator--) | 返回一个枚举器，用于遍历 `Notebook` 的子节点。 |
| [loadChildDocument(InputStream stream)](#loadChildDocument-java.io.InputStream-) | 添加子文档节点。 |
| [loadChildDocument(InputStream stream, LoadOptions loadOptions)](#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-) | 添加子文档节点。 |
| [loadChildDocument(String filePath)](#loadChildDocument-java.lang.String-) | 添加子文档节点。 |
| [loadChildDocument(String filePath, LoadOptions loadOptions)](#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-) | 添加子文档节点。 |
| [loadChildNotebook(String filePath)](#loadChildNotebook-java.lang.String-) | 添加子笔记本节点。 |
| [loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)](#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | 添加子笔记本节点。 |
| [removeChild(INotebookChildNode oldChild)](#removeChild-com.aspose.note.INotebookChildNode-) | 移除子节点。 |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | 将 OneNote 文档保存到流中。 |
| [save(OutputStream stream, NotebookSaveOptions options)](#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-) | 使用指定的保存选项将 OneNote 文档保存到流中。 |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | 以指定格式将 OneNote 文档保存到流中。 |
| [save(String fileName)](#save-java.lang.String-) | 将 OneNote 文档保存到文件。 |
| [save(String fileName, NotebookSaveOptions options)](#save-java.lang.String-com.aspose.note.NotebookSaveOptions-) | 使用指定的保存选项将 OneNote 文档保存到文件。 |
| [save(String fileName, int format)](#save-java.lang.String-int-) | 以指定格式将 OneNote 文档保存到文件。 |
| [setColor(Color value)](#setColor-java.awt.Color-) | 获取或设置颜色。 |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | 获取或设置显示名称。 |
| [setHistoryEnabled(boolean value)](#setHistoryEnabled-boolean-) | 获取或设置一个值，指示是否启用历史记录。 |
### Notebook() {#Notebook--}
```
public Notebook()
```


初始化 `Notebook` 类的新实例。

### Notebook(String filePath) {#Notebook-java.lang.String-}
```
public Notebook(String filePath)
```


初始化 `Notebook` 类的新实例。打开来自文件的现有 OneNote 笔记本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filePath | java.lang.String | 文件路径。 |

### Notebook(String filePath, NotebookLoadOptions loadOptions) {#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public Notebook(String filePath, NotebookLoadOptions loadOptions)
```


初始化 `Notebook` 类的新实例。 从文件打开现有的 OneNote 笔记本。 允许指定附加选项，例如子项加载策略（\"lazy\"/instant）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filePath | java.lang.String | 文件路径。 |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | 加载选项。 |

### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


按节点类型获取所有子节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - 子节点的列表。

`T1`：返回列表中元素的类型。
### appendChild(INotebookChildNode newChild) {#appendChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode appendChild(INotebookChildNode newChild)
```


将节点添加到列表末尾。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| newChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | 要添加的节点。 |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The added node.
### getColor() {#getColor--}
```
public Color getColor()
```


获取或设置颜色。

**Returns:**
java.awt.Color
### getCount() {#getCount--}
```
public int getCount()
```


获取 `Notebook` 中包含的元素数量。

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


获取或设置显示名称。

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

值：GUID。

**Returns:**
java.util.UUID
### getGuidInternal() {#getGuidInternal--}
```
public System.Guid getGuidInternal()
```




**Returns:**
com.aspose.ms.System.Guid
### get_Item(int index) {#get-Item-int-}
```
public INotebookChildNode get_Item(int index)
```


按给定索引获取笔记本子节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| index | int | 子节点的索引。 |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The child node on the `index` position.
### isHistoryEnabled() {#isHistoryEnabled--}
```
public boolean isHistoryEnabled()
```


获取或设置一个值，指示是否启用历史记录。

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<INotebookChildNode> iterator()
```


返回一个枚举器，用于遍历 `Notebook` 的子节点。

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.INotebookChildNode&gt; - 一个 `IEnumerator`。
### loadChildDocument(InputStream stream) {#loadChildDocument-java.io.InputStream-}
```
public void loadChildDocument(InputStream stream)
```


添加子文档节点。 从流中打开现有的 OneNote 文档。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.InputStream | 流。 |

### loadChildDocument(InputStream stream, LoadOptions loadOptions) {#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(InputStream stream, LoadOptions loadOptions)
```


添加子文档节点。 从流中打开现有的 OneNote 文档。 允许指定附加加载选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.InputStream | 流。 |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | 加载选项。 |

### loadChildDocument(String filePath) {#loadChildDocument-java.lang.String-}
```
public void loadChildDocument(String filePath)
```


添加子文档节点。 从文件中打开现有的 OneNote 文档。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filePath | java.lang.String | 文件路径。 |

### loadChildDocument(String filePath, LoadOptions loadOptions) {#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(String filePath, LoadOptions loadOptions)
```


添加子文档节点。 从文件中打开现有的 OneNote 文档。 允许指定附加加载选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filePath | java.lang.String | 文件路径。 |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | 加载选项。 |

### loadChildNotebook(String filePath) {#loadChildNotebook-java.lang.String-}
```
public void loadChildNotebook(String filePath)
```


添加子笔记本节点。 从文件中打开现有的 OneNote 笔记本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filePath | java.lang.String | 文件路径。 |

### loadChildNotebook(String filePath, NotebookLoadOptions loadOptions) {#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public void loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)
```


添加子笔记本节点。 从文件中打开现有的 OneNote 笔记本。 允许指定附加加载选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filePath | java.lang.String | 文件路径。 |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | 加载选项。 |

### removeChild(INotebookChildNode oldChild) {#removeChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode removeChild(INotebookChildNode oldChild)
```


移除子节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| oldChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | 要删除的节点。 |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The removed node.
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


将 OneNote 文档保存到流中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.OutputStream | 流。 |

### save(OutputStream stream, NotebookSaveOptions options) {#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-}
```
public void save(OutputStream stream, NotebookSaveOptions options)
```


使用指定的保存选项将 OneNote 文档保存到流中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.OutputStream | 流。 |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | 指定文档保存的选项。 |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


以指定格式将 OneNote 文档保存到流中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.OutputStream | 流。 |
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

### save(String fileName, NotebookSaveOptions options) {#save-java.lang.String-com.aspose.note.NotebookSaveOptions-}
```
public void save(String fileName, NotebookSaveOptions options)
```


使用指定的保存选项将 OneNote 文档保存到文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文件名 | java.lang.String | 文件的完整名称。如果具有指定完整名称的文件已存在，则会覆盖现有文件。 |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | 指定文档在文件中保存的选项。 |

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

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


获取或设置颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.awt.Color |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


获取或设置显示名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setHistoryEnabled(boolean value) {#setHistoryEnabled-boolean-}
```
public void setHistoryEnabled(boolean value)
```


获取或设置一个值，指示是否启用历史记录。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

