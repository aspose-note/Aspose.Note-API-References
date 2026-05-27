---
title: "Image.Alignment"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية Image. تحصل أو تعين المحاذاة"
type: docs
weight: 20
url: /ar/net/aspose.note/image/alignment/
---
## Image.Alignment property

يحصل أو يعيّن المحاذاة.

```csharp
public HorizontalAlignment Alignment { get; set; }
```

## أمثلة

يظهر كيفية إضافة صورة من ملف إلى مستند مع خصائص محددة من قبل المستخدم.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images();

// تحميل المستند من الدفق.
Document doc = new Document(dataDir + "Aspose.one");

// احصل على الصفحة الأولى من المستند.
Page page = doc.FirstChild;

// تحميل صورة من الملف.
Image image = new Image(dataDir + "image.jpg")
                          {
                              // غيّر حجم الصورة وفقًا لاحتياجاتك (اختياري).
                              Width = 100,
                              Height = 100,

                              // حدد موقع الصورة في الصفحة (اختياري).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // ضبط محاذاة الصورة
                              Alignment = HorizontalAlignment.Right
                          };

// أضف الصورة إلى الصفحة.
page.AppendChildLast(image);
```

يظهر كيفية إضافة صورة من الدفق إلى مستند.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images();

// إنشاء كائن من فئة Document
Document doc = new Document();

// تهيئة كائن فئة Page
Page page = new Page();

Outline outline1 = new Outline();
OutlineElement outlineElem1 = new OutlineElement();

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // تحميل الصورة الثانية باستخدام اسم الصورة، الامتداد، والدفق.
    Image image1 = new Image("Penguins.jpg", fs)
                                   {
                                       // ضبط محاذاة الصورة
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// حفظ مستند OneNote.
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

يظهر كيفية إضافة صورة من ملف إلى مستند.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images();

// إنشاء كائن من فئة Document
Document doc = new Document();

// تهيئة كائن فئة Page
Page page = new Page();

// تهيئة كائن فئة Outline وتعيين خصائص الإزاحة
Outline outline = new Outline();

// تهيئة كائن فئة OutlineElement
OutlineElement outlineElem = new OutlineElement();

// تحميل صورة عبر مسار الملف.
Image image = new Image(dataDir + "image.jpg")
                          {
                              // ضبط محاذاة الصورة
                              Alignment = HorizontalAlignment.Right
                          };

// إضافة صورة
outlineElem.AppendChildLast(image);

// إضافة عناصر المخطط
outline.AppendChildLast(outlineElem);

// إضافة عقدة المخطط
page.AppendChildLast(outline);

// إضافة عقدة الصفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote.
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

### انظر أيضًا

* enum [HorizontalAlignment](../../horizontalalignment/)
* class [Image](../)
* namespace [Aspose.Note](../../image/)
* assembly [Aspose.Note](../../../)


