---
title: "Image.Height"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية Image. تحصل أو تعين الارتفاع. هذا هو الارتفاع الحقيقي للصورة في مستند MS OneNote"
type: docs
weight: 90
url: /ar/net/aspose.note/image/height/
---
## Image.Height property

يحصل أو يعيّن الارتفاع. هذا هو الارتفاع الحقيقي للصورة في مستند MS OneNote.

```csharp
public float Height { get; set; }
```

## أمثلة

يظهر كيفية الحصول على معلومات ميتا للصورة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// الحصول على جميع عقد Image
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

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


