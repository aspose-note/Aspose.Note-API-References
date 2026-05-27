---
title: "Page.Clone"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "طريقة Page. تنسخ الصفحة"
type: docs
weight: 140
url: /ar/net/aspose.note/page/clone/
---
## Page.Clone method

ينسخ الصفحة.

```csharp
public Page Clone(bool cloneHistory = false)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cloneHistory | Boolean | يحدد ما إذا كان يجب نسخ سجل الصفحة.. |

### قيمة الإرجاع

نسخة من الصفحة.

## أمثلة

يعرض كيفية دفع النسخة الحالية من الصفحة إلى السجل.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// تحميل مستند OneNote والحصول على العنصر الفرعي الأول.
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.Add(page.Clone());

document.Save(dataDir + "PushCurrentPageVersion_out.one");
```

يعرض كيفية استنساخ صفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// تحميل مستند OneNote.
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// استنساخ إلى مستند جديد بدون تاريخ
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// استنساخ إلى مستند جديد مع التاريخ
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

### انظر أيضًا

* class [Page](../)
* namespace [Aspose.Note](../../page/)
* assembly [Aspose.Note](../../../)


