---
title: "Image.AlternativeTextDescription"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية Image. تحصل أو تعين نص بديل للجسم للصورة"
type: docs
weight: 30
url: /ar/net/aspose.note/image/alternativetextdescription/
---
## Image.AlternativeTextDescription property

يحصل أو يعيّن نصًا بديلًا للجسم للصورة.

```csharp
public string AlternativeTextDescription { get; set; }
```

## أمثلة

يظهر كيفية تعيين وصف نصي لصورة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images();

var document = new Document();
var page = new Page();
var image = new Image(dataDir + "image.jpg")
            {
                AlternativeTextTitle = "This is an image's title!",
                AlternativeTextDescription = "And this is an image's description!"
            };
page.AppendChildLast(image);
document.AppendChildLast(page);

dataDir = dataDir + "ImageAlternativeText_out.one";
document.Save(dataDir);
```

### انظر أيضًا

* class [Image](../)
* namespace [Aspose.Note](../../image/)
* assembly [Aspose.Note](../../../)


