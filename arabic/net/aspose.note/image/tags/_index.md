---
title: "Image.Tags"
second_title: "مرجع API لـ Aspose.Note لـ .NET"
description: "خاصية Image. تحصل على قائمة بجميع وسوم الفقرة"
type: docs
weight: 160
url: /ar/net/aspose.note/image/tags/
---
## Image.Tags property

يحصل على قائمة بجميع العلامات في الفقرة.

```csharp
public List<ITag> Tags { get; }
```

## أمثلة

يوضح كيفية إضافة صورة جديدة مع علامة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tags();

// إنشاء كائن من الفئة Document
Document doc = new Document();

// تهيئة كائن الفئة Page
Page page = new Page();

// تهيئة كائن الفئة Outline
Outline outline = new Outline();

// تهيئة كائن الفئة OutlineElement
OutlineElement outlineElem = new OutlineElement();

// تحميل صورة
Image image = new Image(dataDir + "icon.jpg");

// إدراج صورة في عقدة المستند
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// إضافة عقدة عنصر المخطط
outline.AppendChildLast(outlineElem);

// إضافة عقدة المخطط
page.AppendChildLast(outline);

// إضافة عقدة الصفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
```

### انظر أيضًا

* interface [ITag](../../itag/)
* class [Image](../)
* namespace [Aspose.Note](../../image/)
* assembly [Aspose.Note](../../../)


