---
title: Image.Tags
second_title: Aspose.Note لمرجع NET API
description: Image ملكية. يحصل على قائمة بكافة علامات الفقرة .
type: docs
weight: 160
url: /ar/net/aspose.note/image/tags/
---
## Image.Tags property

يحصل على قائمة بكافة علامات الفقرة .

```csharp
public List<ITag> Tags { get; }
```

### أمثلة

يوضح كيفية إضافة صورة جديدة مع علامة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tags();

// إنشاء كائن من فئة المستند
Document doc = new Document();

// تهيئة كائن فئة الصفحة
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// تهيئة كائن فئة المخطط التفصيلي
Outline outline = new Outline(doc);

// تهيئة كائن فئة OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// تحميل صورة
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

// أدخل الصورة في عقدة المستند
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// إضافة عقدة عنصر المخطط التفصيلي
outline.AppendChildLast(outlineElem);

// إضافة عقدة المخطط التفصيلي
page.AppendChildLast(outline);

// إضافة عقدة الصفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
```

### أنظر أيضا

* interface [ITag](../../itag/)
* class [Image](../)
* مساحة الاسم [Aspose.Note](../../image/)
* المجسم [Aspose.Note](../../../)


