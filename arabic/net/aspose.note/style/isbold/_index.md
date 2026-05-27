---
title: "Style.IsBold"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية Style. يحصل على أو يضبط قيمة تشير إلى ما إذا كان نمط النص عريض"
type: docs
weight: 60
url: /ar/net/aspose.note/style/isbold/
---
## Style.IsBold property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان نمط النص غامقًا.

```csharp
public bool IsBold { get; set; }
```

## أمثلة

دعنا نبرز عناوين الصفحة بين العناوين الأخرى بزيادة حجم الخط.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// حمّل المستند إلى Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// تكرار عبر عناوين الصفحة.
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

دعنا نبرز تغييرات النص الأخيرة عن طريق التظليل.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// حمّل المستند إلى Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// احصل على عقد RichText المعدلة الأسبوع الماضي.
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

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Note](../../style/)
* assembly [Aspose.Note](../../../)


