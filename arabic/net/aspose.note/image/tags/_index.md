---
title: "Image.Tags"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية Image. تحصل على قائمة بجميع العلامات في الفقرة"
type: docs
weight: 160
url: /ar/net/aspose.note/image/tags/
---
## Image.Tags property

يحصل على قائمة جميع العلامات في الفقرة.

```csharp
public List<ITag> Tags { get; }
```

## أمثلة

يعرض كيفية إضافة صورة جديدة مع علامة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tags();

// إنشاء كائن من فئة Document
Document doc = new Document();

// تهيئة كائن فئة Page
Page page = new Page();

// تهيئة كائن فئة Outline
Outline outline = new Outline();

// تهيئة كائن فئة OutlineElement
OutlineElement outlineElem = new OutlineElement();

// تحميل صورة.
Image image = new Image(dataDir + "icon.jpg");

// إدراج صورة في عقدة المستند.
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// إضافة عقدة عنصر المخطط
outline.AppendChildLast(outlineElem);

// إضافة عقدة المخطط
page.AppendChildLast(outline);

// إضافة عقدة صفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote.
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
```

### انظر أيضًا

* interface [ITag](../../itag/)
* class [Image](../)
* namespace [Aspose.Note](../../image/)
* assembly [Aspose.Note](../../../)


