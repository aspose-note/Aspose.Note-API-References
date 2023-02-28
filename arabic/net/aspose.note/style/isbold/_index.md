---
title: Style.IsBold
second_title: Aspose.Note لمرجع NET API
description: Style ملكية. الحصول على أو تعيين قيمة تشير إلى ما إذا كان نمط النص غامقًا .
type: docs
weight: 60
url: /ar/net/aspose.note/style/isbold/
---
## Style.IsBold property

الحصول على أو تعيين قيمة تشير إلى ما إذا كان نمط النص غامقًا .

```csharp
public bool IsBold { get; set; }
```

### أمثلة

دعنا نبرز عناوين الصفحة بين الرؤوس الأخرى عن طريق زيادة حجم الخط.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// قم بتحميل المستند في Aspose.
Document document = new Document(dataDir + "Aspose.one");

// تكرار من خلال عناوين الصفحة.
foreach (var title in document.Select(e => e.Title.TitleText))
{
    title.ParagraphStyle.FontSize = 24;
    title.ParagraphStyle.IsBold = true;

    foreach (var run in title.TextRuns)
    {
        run.Style.FontSize = 24;
        run.Style.IsBold = true;
    }
}

document.Save(Path.Combine(dataDir, "ChangePageTitleStyle.pdf"));
```

دعنا نؤكد على التغييرات الأخيرة في النص من خلال التمييز.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// قم بتحميل المستند في Aspose.
Document document = new Document(dataDir + "Aspose.one");

// Get RichText عُدلت الأسبوع الماضي.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // تعيين لون التظليل
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // تعيين لون التظليل
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

### أنظر أيضا

* class [Style](../)
* مساحة الاسم [Aspose.Note](../../style/)
* المجسم [Aspose.Note](../../../)


