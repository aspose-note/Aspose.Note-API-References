---
title: "NotebookLoadOptions"
second_title: "Aspose.Note for Java API 参考"
description: "用于加载笔记本的选项。"
type: docs
weight: 58
url: /zh/java/com.aspose.note/notebookloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class NotebookLoadOptions
```

用于加载笔记本的选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [NotebookLoadOptions()](#NotebookLoadOptions--) | 初始化 `NotebookLoadOptions` 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getDeferredLoading()](#getDeferredLoading--) | 获取或设置一个值，指示是否应在以后显式加载子文档。 |
| [getInstantLoading()](#getInstantLoading--) | 获取或设置一个值，指示是否应在父文档加载时加载子文档。 |
| [setDeferredLoading(boolean value)](#setDeferredLoading-boolean-) | 获取或设置一个值，指示是否应在以后显式加载子文档。 |
| [setInstantLoading(boolean value)](#setInstantLoading-boolean-) | 获取或设置一个值，指示是否应在父文档加载时加载子文档。 |
### NotebookLoadOptions() {#NotebookLoadOptions--}
```
public NotebookLoadOptions()
```


初始化 `NotebookLoadOptions` 类的新实例。

### getDeferredLoading() {#getDeferredLoading--}
```
public final boolean getDeferredLoading()
```


获取或设置一个值，指示是否应在以后显式加载子文档。

--------------------

默认值为 `false`，因此子文档将被隐式加载。值为 `true` 表示用户应调用 `Notebook.loadChildDocument`，或在笔记本本身加载后对每个笔记本的子节点进行调用。如果值为 `true`，`NotebookLoadOptions.instantLoading` 选项将被忽略。如果笔记本是从流中加载的，无论用户是否显式设置为 `false`，该值始终为 `true`。

**Returns:**
boolean
### getInstantLoading() {#getInstantLoading--}
```
public boolean getInstantLoading()
```


获取或设置一个值，指示是否应在父文档加载时加载子文档。

--------------------

默认值为 `false`，因此子文档将被 \"懒惰\" 加载，即它们的加载应推迟到直接访问特定子文档时。值为 `true` 表示应立即加载它们。

**Returns:**
boolean
### setDeferredLoading(boolean value) {#setDeferredLoading-boolean-}
```
public final void setDeferredLoading(boolean value)
```


获取或设置一个值，指示是否应在以后显式加载子文档。

--------------------

默认值为 `false`，因此子文档将被隐式加载。值为 `true` 表示用户应调用 `Notebook.loadChildDocument`，或在笔记本本身加载后对每个笔记本的子节点进行调用。如果值为 `true`，`NotebookLoadOptions.instantLoading` 选项将被忽略。如果笔记本是从流中加载的，无论用户是否显式设置为 `false`，该值始终为 `true`。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setInstantLoading(boolean value) {#setInstantLoading-boolean-}
```
public void setInstantLoading(boolean value)
```


获取或设置一个值，指示是否应在父文档加载时加载子文档。

--------------------

默认值为 `false`，因此子文档将被 \"懒惰\" 加载，即它们的加载应推迟到直接访问特定子文档时。值为 `true` 表示应立即加载它们。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

