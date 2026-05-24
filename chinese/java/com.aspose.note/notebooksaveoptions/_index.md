---
title: "NotebookSaveOptions"
second_title: "Aspose.Note for Java API 参考"
description: "表示特定格式的笔记本保存选项的抽象基类。"
type: docs
weight: 61
url: /zh/java/com.aspose.note/notebooksaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class NotebookSaveOptions
```

表示特定格式的笔记本保存选项的抽象基类。
## 方法

| 方法 | 描述 |
| --- | --- |
| [getDeferredSaving()](#getDeferredSaving--) | 获取或设置一个值，指示是否应显式保存子文档。 |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | 获取所有笔记本子文档的保存选项。 |
| [getFlatten()](#getFlatten--) | 获取或设置一个值，指示是否将笔记本子层次结构保存为扁平化。 |
| [getSaveFormat()](#getSaveFormat--) | 获取笔记本保存的格式。 |
| [setDeferredSaving(boolean value)](#setDeferredSaving-boolean-) | 获取或设置一个值，指示是否应显式保存子文档。 |
| [setFlatten(boolean value)](#setFlatten-boolean-) | 获取或设置一个值，指示是否将笔记本子层次结构保存为扁平化。 |
### getDeferredSaving() {#getDeferredSaving--}
```
public boolean getDeferredSaving()
```


获取或设置一个值，指示是否应显式保存子文档。

--------------------

默认值为 `false`，因此子文档将隐式保存。值为 `true` 表示用户应显式保存每个笔记本的子节点。如果笔记本保存到流中，无论用户是否显式设置为 `false`，该值始终为 `true`。

**Returns:**
boolean
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public abstract SaveOptions getDocumentSaveOptionsInternal()
```


获取所有笔记本子文档的保存选项。

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getFlatten() {#getFlatten--}
```
public boolean getFlatten()
```


获取或设置一个值，指示是否将笔记本子层次结构保存为扁平化。

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public abstract int getSaveFormat()
```


获取笔记本保存的格式。

**Returns:**
int
### setDeferredSaving(boolean value) {#setDeferredSaving-boolean-}
```
public void setDeferredSaving(boolean value)
```


获取或设置一个值，指示是否应显式保存子文档。

--------------------

默认值为 `false`，因此子文档将隐式保存。值为 `true` 表示用户应显式保存每个笔记本的子节点。如果笔记本保存到流中，无论用户是否显式设置为 `false`，该值始终为 `true`。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFlatten(boolean value) {#setFlatten-boolean-}
```
public void setFlatten(boolean value)
```


获取或设置一个值，指示是否将笔记本子层次结构保存为扁平化。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

