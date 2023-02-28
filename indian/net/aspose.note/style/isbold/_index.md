---
title: Style.IsBold
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Style संपत्त. एक मन प्रप्त य सेट करत है ज इंगत करत है क टेक्स्ट शैल बल्ड है य नहं
type: docs
weight: 60
url: /hi/net/aspose.note/style/isbold/
---
## Style.IsBold property

एक मान प्राप्त या सेट करता है जो इंगित करता है कि टेक्स्ट शैली बोल्ड है या नहीं।

```csharp
public bool IsBold { get; set; }
```

### उदाहरण

फ़ॉन्ट का आकार बढ़ाकर अन्य शीर्षकों के बीच पृष्ठ के शीर्षक पर जोर दें।

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document document = new Document(dataDir + "Aspose.one");

// पृष्ठ के शीर्षकों के माध्यम से पुनरावृति करें।
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

* class [Style](../)
* नाम स्थान [Aspose.Note](../../style/)
* सभा [Aspose.Note](../../../)


