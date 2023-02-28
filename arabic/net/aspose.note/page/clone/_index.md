---
title: Page.Clone
second_title: Aspose.Note لمرجع NET API
description: Page طريقة. استنساخ الصفحة .
type: docs
weight: 140
url: /ar/net/aspose.note/page/clone/
---
## Page.Clone method

استنساخ الصفحة .

```csharp
public Page Clone(bool cloneHistory = false)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| cloneHistory | Boolean | تحديد ما إذا كان يجب نسخ محفوظات الصفحة .. |

### قيمة الإرجاع

نسخة من الصفحة .

### أمثلة

يوضح كيفية دفع الإصدار الحالي من الصفحة إلى المحفوظات.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// قم بتحميل مستند OneNote واحصل على الطفل الأول           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.Add(page.Clone());

document.Save(dataDir + "PushCurrentPageVersion_out.one");
```

يوضح كيفية استنساخ الصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// تحميل مستند OneNote
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// استنساخ في مستند جديد بدون محفوظات
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// استنساخ في مستند جديد مع المحفوظات
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

### أنظر أيضا

* class [Page](../)
* مساحة الاسم [Aspose.Note](../../page/)
* المجسم [Aspose.Note](../../../)


