---
title: "NotebookSaveOptionsGeneric"
second_title: "مرجع Aspose.Note for Java API"
description: "فئة أساسية مجردة تمثل خيارات حفظ دفتر الملاحظات لتنسيق معين وتوفر خيارات حفظ مشتركة لجميع العقد الفرعية للمستند."
type: docs
weight: 62
url: /ar/java/com.aspose.note/notebooksaveoptionsgeneric/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions)
```
public abstract class NotebookSaveOptionsGeneric<TDocumentSaveOptions> extends NotebookSaveOptions
```

فئة أساسية مجردة تمثل خيارات حفظ دفتر الملاحظات لتنسيق معين وتوفر خيارات حفظ مشتركة لجميع العقد الفرعية للمستند.

`TDocumentSaveOptions`: خيارات الحفظ لجميع المستندات الفرعية في الدفتر.

TDocumentSaveOptions :
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [NotebookSaveOptionsGeneric()](#NotebookSaveOptionsGeneric--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getDocumentSaveOptions()](#getDocumentSaveOptions--) | يحصل أو يعيّن خيارات الحفظ لجميع المستندات الفرعية في الدفتر. |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | يحصل على خيارات الحفظ لجميع مستندات الأطفال في الدفتر. |
| [getSaveFormat()](#getSaveFormat--) | يحصل على الصيغة التي يُحفظ بها الدفتر. |
### NotebookSaveOptionsGeneric() {#NotebookSaveOptionsGeneric--}
```
public NotebookSaveOptionsGeneric()
```


### getDocumentSaveOptions() {#getDocumentSaveOptions--}
```
public TDocumentSaveOptions getDocumentSaveOptions()
```


يحصل أو يعيّن خيارات الحفظ لجميع المستندات الفرعية في الدفتر.

**Returns:**
TDocumentSaveOptions
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public SaveOptions getDocumentSaveOptionsInternal()
```


يحصل على خيارات الحفظ لجميع مستندات الأطفال في الدفتر.

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


يحصل على الصيغة التي يُحفظ بها الدفتر.

**Returns:**
int
