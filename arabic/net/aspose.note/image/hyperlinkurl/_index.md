---
title: Image.HyperlinkUrl
second_title: Aspose.Note لمرجع NET API
description: Image ملكية. الحصول على أو تعيين الارتباط التشعبي المرتبط بالصورة.
type: docs
weight: 110
url: /ar/net/aspose.note/image/hyperlinkurl/
---
## Image.HyperlinkUrl property

الحصول على أو تعيين الارتباط التشعبي المرتبط بالصورة.

```csharp
public string HyperlinkUrl { get; set; }
```

### أمثلة

يوضح كيفية ربط ارتباط تشعبي بصورة ما.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://image.com "} ;

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

### أنظر أيضا

* class [Image](../)
* مساحة الاسم [Aspose.Note](../../image/)
* المجسم [Aspose.Note](../../../)


