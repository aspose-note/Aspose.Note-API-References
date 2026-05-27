---
title: "Notebook.LoadChildDocument"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "طريقة Notebook. تضيف عقدة مستند طفل. تفتح مستند OneNote موجود من ملف"
type: docs
weight: 120
url: /ar/net/aspose.note/notebook/loadchilddocument/
---
## LoadChildDocument(string) {#loadchilddocument_2}

يضيف عقدة مستند طفل. يفتح مستند OneNote موجود من ملف.

```csharp
public void LoadChildDocument(string filePath)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | String | مسار الملف. |

## أمثلة

يوضح كيفية تحميل الدفتر من تدفق.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notebook.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

### انظر أيضًا

* class [Notebook](../)
* namespace [Aspose.Note](../../notebook/)
* assembly [Aspose.Note](../../../)

---

## LoadChildDocument(string, LoadOptions) {#loadchilddocument_3}

يضيف عقدة مستند طفل. يفتح مستند OneNote موجود من ملف. يسمح بتحديد خيارات تحميل إضافية.

```csharp
public void LoadChildDocument(string filePath, LoadOptions loadOptions)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | String | مسار الملف. |
| loadOptions | LoadOptions | خيارات التحميل. |

### انظر أيضًا

* class [LoadOptions](../../loadoptions/)
* class [Notebook](../)
* namespace [Aspose.Note](../../notebook/)
* assembly [Aspose.Note](../../../)

---

## LoadChildDocument(Stream) {#loadchilddocument}

يضيف عقدة مستند طفل. يفتح مستند OneNote موجود من تدفق.

```csharp
public void LoadChildDocument(Stream stream)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| دفق | Stream | التدفق. |

## أمثلة

يوضح كيفية تحميل الدفتر من تدفق.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notebook.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

### انظر أيضًا

* class [Notebook](../)
* namespace [Aspose.Note](../../notebook/)
* assembly [Aspose.Note](../../../)

---

## LoadChildDocument(Stream, LoadOptions) {#loadchilddocument_1}

يضيف عقدة مستند طفل. يفتح مستند OneNote موجود من تدفق. يسمح بتحديد خيارات تحميل إضافية.

```csharp
public void LoadChildDocument(Stream stream, LoadOptions loadOptions)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| دفق | Stream | التدفق. |
| loadOptions | LoadOptions | خيارات التحميل. |

### انظر أيضًا

* class [LoadOptions](../../loadoptions/)
* class [Notebook](../)
* namespace [Aspose.Note](../../notebook/)
* assembly [Aspose.Note](../../../)


