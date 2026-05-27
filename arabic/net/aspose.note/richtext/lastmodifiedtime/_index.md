---
title: "RichText.LastModifiedTime"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية RichText. تحصل أو تعيّن وقت التعديل الأخير"
type: docs
weight: 60
url: /ar/net/aspose.note/richtext/lastmodifiedtime/
---
## RichText.LastModifiedTime property

يحصل أو يعيّن وقت آخر تعديل.

```csharp
public DateTime LastModifiedTime { get; set; }
```

## أمثلة

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

* class [RichText](../)
* namespace [Aspose.Note](../../richtext/)
* assembly [Aspose.Note](../../../)


