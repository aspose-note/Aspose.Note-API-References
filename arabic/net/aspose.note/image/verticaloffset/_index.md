---
title: Image.VerticalOffset
second_title: Aspose.Note لمرجع NET API
description: Image ملكية. الحصول على أو تعيين الإزاحة الرأسية .
type: docs
weight: 170
url: /ar/net/aspose.note/image/verticaloffset/
---
## Image.VerticalOffset property

الحصول على أو تعيين الإزاحة الرأسية .

```csharp
public float VerticalOffset { get; set; }
```

### أمثلة

يوضح كيفية إضافة صورة من ملف إلى مستند بخصائص يحددها المستخدم.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images();

// تحميل المستند من الدفق.
Document doc = new Document(dataDir + "Aspose.one");

// احصل على الصفحة الأولى من المستند.
Aspose.Note.Page page = doc.FirstChild;

// تحميل صورة من الملف.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // قم بتغيير حجم الصورة وفقًا لاحتياجاتك (اختياري).
                              Width = 100,
                              Height = 100,

                              // تعيين موقع الصورة في الصفحة (اختياري).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // تعيين محاذاة الصورة
                              Alignment = HorizontalAlignment.Right
                          };

// أضف الصورة إلى الصفحة.
page.AppendChildLast(image);
```

### أنظر أيضا

* class [Image](../)
* مساحة الاسم [Aspose.Note](../../image/)
* المجسم [Aspose.Note](../../../)


