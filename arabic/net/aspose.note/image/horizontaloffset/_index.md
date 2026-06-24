---
title: "Image.HorizontalOffset"
second_title: "مرجع API لـ Aspose.Note لـ .NET"
description: "خاصية Image. تحصل أو تعين الإزاحة الأفقية"
type: docs
weight: 100
url: /ar/net/aspose.note/image/horizontaloffset/
---
## Image.HorizontalOffset property

يحصل أو يعيّن الإزاحة الأفقية.

```csharp
public float HorizontalOffset { get; set; }
```

## أمثلة

يعرض كيفية إضافة صورة من ملف إلى مستند مع خصائص معرفة من قبل المستخدم.

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

                              // تعيين محاذاة الصورة
                              Alignment = HorizontalAlignment.Right
                          };

// أضف الصورة إلى الصفحة.
page.AppendChildLast(image);
```

### انظر أيضًا

* class [Image](../)
* namespace [Aspose.Note](../../image/)
* assembly [Aspose.Note](../../../)


