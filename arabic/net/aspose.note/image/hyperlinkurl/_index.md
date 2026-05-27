---
title: "Image.HyperlinkUrl"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية Image. تحصل أو تعين الارتباط التشعبي المرتبط بالصورة"
type: docs
weight: 110
url: /ar/net/aspose.note/image/hyperlinkurl/
---
## Image.HyperlinkUrl property

يحصل أو يعيّن الرابط التشعبي المرتبط بالصورة.

```csharp
public string HyperlinkUrl { get; set; }
```

## أمثلة

يعرض كيفية ربط ارتباط تشعبي بصورة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page();

var image = new Image(dataDir + "image.jpg") { HyperlinkUrl = "https://image.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

### انظر أيضًا

* class [Image](../)
* namespace [Aspose.Note](../../image/)
* assembly [Aspose.Note](../../../)


