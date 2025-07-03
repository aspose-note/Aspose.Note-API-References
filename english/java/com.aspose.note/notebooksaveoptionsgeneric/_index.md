---
title: NotebookSaveOptionsGeneric
second_title: Aspose.Note for Java API Reference
description: An abstract base class which represents notebook saving options for a particular format and provides common saving options for all document child nodes.
type: docs
weight: 62
url: /java/com.aspose.note/notebooksaveoptionsgeneric/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions)
```
public abstract class NotebookSaveOptionsGeneric<TDocumentSaveOptions> extends NotebookSaveOptions
```

An abstract base class which represents notebook saving options for a particular format and provides common saving options for all document child nodes.

`TDocumentSaveOptions`: The save options for all notebook's child documents.

 TDocumentSaveOptions : 
## Constructors

| Constructor | Description |
| --- | --- |
| [NotebookSaveOptionsGeneric()](#NotebookSaveOptionsGeneric--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getDocumentSaveOptions()](#getDocumentSaveOptions--) | Gets or sets the save options for all notebook's child documents. |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | Gets the save options for all notebook's child documents. |
| [getSaveFormat()](#getSaveFormat--) | Gets the format in which the notebook is saved. |
### NotebookSaveOptionsGeneric() {#NotebookSaveOptionsGeneric--}
```
public NotebookSaveOptionsGeneric()
```


### getDocumentSaveOptions() {#getDocumentSaveOptions--}
```
public TDocumentSaveOptions getDocumentSaveOptions()
```


Gets or sets the save options for all notebook's child documents.

**Returns:**
TDocumentSaveOptions
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public SaveOptions getDocumentSaveOptionsInternal()
```


Gets the save options for all notebook's child documents.

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Gets the format in which the notebook is saved.

**Returns:**
int
