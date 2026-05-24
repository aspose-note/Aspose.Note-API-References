---
title: "NotebookSaveOptionsGeneric"
second_title: "Aspose.Note for Java API 参考"
description: "表示特定格式的笔记本保存选项并为所有文档子节点提供通用保存选项的抽象基类。"
type: docs
weight: 62
url: /zh/java/com.aspose.note/notebooksaveoptionsgeneric/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions)
```
public abstract class NotebookSaveOptionsGeneric<TDocumentSaveOptions> extends NotebookSaveOptions
```

表示特定格式的笔记本保存选项并为所有文档子节点提供通用保存选项的抽象基类。

`TDocumentSaveOptions`: 所有笔记本子文档的保存选项。

TDocumentSaveOptions :
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [NotebookSaveOptionsGeneric()](#NotebookSaveOptionsGeneric--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getDocumentSaveOptions()](#getDocumentSaveOptions--) | 获取或设置所有笔记本子文档的保存选项。 |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | 获取所有笔记本子文档的保存选项。 |
| [getSaveFormat()](#getSaveFormat--) | 获取笔记本保存的格式。 |
### NotebookSaveOptionsGeneric() {#NotebookSaveOptionsGeneric--}
```
public NotebookSaveOptionsGeneric()
```


### getDocumentSaveOptions() {#getDocumentSaveOptions--}
```
public TDocumentSaveOptions getDocumentSaveOptions()
```


获取或设置所有笔记本子文档的保存选项。

**Returns:**
TDocumentSaveOptions
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public SaveOptions getDocumentSaveOptionsInternal()
```


获取所有笔记本子文档的保存选项。

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


获取笔记本保存的格式。

**Returns:**
int
