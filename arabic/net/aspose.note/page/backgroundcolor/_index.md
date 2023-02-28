---
title: Page.BackgroundColor
second_title: Aspose.Note لمرجع NET API
description: Page ملكية. الحصول على لون خلفية الصفحة أو تعيينه.
type: docs
weight: 30
url: /ar/net/aspose.note/page/backgroundcolor/
---
## Page.BackgroundColor property

الحصول على لون خلفية الصفحة أو تعيينه.

```csharp
public Color BackgroundColor { get; set; }
```

### أمثلة

يوضح كيفية تعيين لون خلفية الصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// قم بتحميل مستند OneNote واحصل على الطفل الأول           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in document)
{
    page.BackgroundColor = Color.BlueViolet;
}

document.Save(Path.Combine(dataDir, "SetPageBackgroundColor.one"));
```

يوضح كيفية تطبيق نمط النسق الداكن على مستند.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Text();

// قم بتحميل المستند في Aspose.
Document doc = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in doc)
{
    page.BackgroundColor = Color.Black;
}

foreach (var node in doc.GetChildNodes<RichText>())
{
    var c = node.ParagraphStyle.FontColor;
    if (c.IsEmpty || Math.Abs(c.R - Color.Black.R) + Math.Abs(c.G - Color.Black.G) + Math.Abs(c.B - Color.Black.B) <= 30)
    {
        node.ParagraphStyle.FontColor = Color.White;
    }
}

doc.Save(Path.Combine(dataDir, "AsposeDarkTheme.pdf"));
```

### أنظر أيضا

* class [Page](../)
* مساحة الاسم [Aspose.Note](../../page/)
* المجسم [Aspose.Note](../../../)


