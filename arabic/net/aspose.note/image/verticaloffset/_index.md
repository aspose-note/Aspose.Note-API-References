---
title: "Image.VerticalOffset"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية Image. يحصل أو يضبط الإزاحة العمودية"
type: docs
weight: 170
url: /ar/net/aspose.note/image/verticaloffset/
---
## Image.VerticalOffset property

يحصل أو يضبط الإزاحة العمودية.

```csharp
public float VerticalOffset { get; set; }
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

### انظر أيضًا

* class [Image](../)
* namespace [Aspose.Note](../../image/)
* assembly [Aspose.Note](../../../)


