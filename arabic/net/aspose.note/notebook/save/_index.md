---
title: "Notebook.Save"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "طريقة Notebook. تحفظ مستند OneNote إلى ملف"
type: docs
weight: 150
url: /ar/net/aspose.note/notebook/save/
---
## Save(string) {#save_3}

يحفظ مستند OneNote إلى ملف.

```csharp
public void Save(string fileName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | String | الاسم الكامل للملف. إذا كان هناك ملف بالاسم الكامل المحدد موجود بالفعل، يتم استبدال الملف الموجود. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | هيكل المستند ينتهك المواصفات. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | تنسيق الحفظ المطلوب غير مدعوم. |

### انظر أيضًا

* class [Notebook](../)
* namespace [Aspose.Note](../../notebook/)
* assembly [Aspose.Note](../../../)

---

## Save(Stream) {#save}

يحفظ مستند OneNote إلى تدفق.

```csharp
public void Save(Stream stream)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| دفق | Stream | التدفق. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | هيكل المستند ينتهك المواصفات. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | تنسيق الحفظ المطلوب غير مدعوم. |

### انظر أيضًا

* class [Notebook](../)
* namespace [Aspose.Note](../../notebook/)
* assembly [Aspose.Note](../../../)

---

## Save(string, SaveFormat) {#save_4}

يحفظ مستند OneNote إلى ملف بالتنسيق المحدد.

```csharp
public void Save(string fileName, SaveFormat format)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | String | الاسم الكامل للملف. إذا كان هناك ملف بالاسم الكامل المحدد موجود بالفعل، يتم استبدال الملف الموجود. |
| تنسيق | SaveFormat | التنسيق الذي سيتم حفظ المستند به. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | هيكل المستند ينتهك المواصفات. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | تنسيق الحفظ المطلوب غير مدعوم. |

### انظر أيضًا

* enum [SaveFormat](../../saveformat/)
* class [Notebook](../)
* namespace [Aspose.Note](../../notebook/)
* assembly [Aspose.Note](../../../)

---

## Save(Stream, SaveFormat) {#save_1}

يحفظ مستند OneNote إلى تدفق بالتنسيق المحدد.

```csharp
public void Save(Stream stream, SaveFormat format)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| دفق | Stream | التدفق. |
| تنسيق | SaveFormat | التنسيق الذي سيتم حفظ المستند به. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | هيكل المستند ينتهك المواصفات. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | تنسيق الحفظ المطلوب غير مدعوم. |

### انظر أيضًا

* enum [SaveFormat](../../saveformat/)
* class [Notebook](../)
* namespace [Aspose.Note](../../notebook/)
* assembly [Aspose.Note](../../../)

---

## Save(string, NotebookSaveOptions) {#save_5}

يحفظ مستند OneNote إلى ملف باستخدام خيارات الحفظ المحددة.

```csharp
public void Save(string fileName, NotebookSaveOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | String | الاسم الكامل للملف. إذا كان هناك ملف بالاسم الكامل المحدد موجود بالفعل، يتم استبدال الملف الموجود. |
| خيارات | NotebookSaveOptions | يحدد الخيارات التي يتم حفظ المستند بها في الملف. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | هيكل المستند ينتهك المواصفات. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | تنسيق الحفظ المطلوب غير مدعوم. |

### انظر أيضًا

* class [NotebookSaveOptions](../../../aspose.note.saving/notebooksaveoptions/)
* class [Notebook](../)
* namespace [Aspose.Note](../../notebook/)
* assembly [Aspose.Note](../../../)

---

## Save(Stream, NotebookSaveOptions) {#save_2}

يحفظ مستند OneNote إلى تدفق باستخدام خيارات الحفظ المحددة.

```csharp
public void Save(Stream stream, NotebookSaveOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| دفق | Stream | التدفق. |
| خيارات | NotebookSaveOptions | يحدد الخيارات التي يتم حفظ المستند بها. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | هيكل المستند ينتهك المواصفات. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | تنسيق الحفظ المطلوب غير مدعوم. |

### انظر أيضًا

* class [NotebookSaveOptions](../../../aspose.note.saving/notebooksaveoptions/)
* class [Notebook](../)
* namespace [Aspose.Note](../../notebook/)
* assembly [Aspose.Note](../../../)


