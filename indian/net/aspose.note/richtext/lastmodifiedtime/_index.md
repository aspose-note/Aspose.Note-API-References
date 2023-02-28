---
title: RichText.LastModifiedTime
second_title: Aspose.Note .NET API संदर्भ के लिए
description: RichText संपत्त. अंतम संशधत समय प्रप्त य सेट करत है
type: docs
weight: 30
url: /hi/net/aspose.note/richtext/lastmodifiedtime/
---
## RichText.LastModifiedTime property

अंतिम संशोधित समय प्राप्त या सेट करता है।

```csharp
public DateTime LastModifiedTime { get; set; }
```

### उदाहरण

हाइलाइट करके नवीनतम टेक्स्ट के परिवर्तनों पर जोर दें।

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document document = new Document(dataDir + "Aspose.one");

// RichText नोड्स को पिछले सप्ताह संशोधित करें।
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // हाइलाइट रंग सेट करें
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // हाइलाइट रंग सेट करें
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

### यह सभी देखें

* class [RichText](../)
* नाम स्थान [Aspose.Note](../../richtext/)
* सभा [Aspose.Note](../../../)


