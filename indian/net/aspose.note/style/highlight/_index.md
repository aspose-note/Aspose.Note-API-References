---
title: Style.Highlight
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Style संपत्त. हइलइट रंग प्रप्त य सेट करत है
type: docs
weight: 50
url: /hi/net/aspose.note/style/highlight/
---
## Style.Highlight property

हाइलाइट रंग प्राप्त या सेट करता है।

```csharp
public Color Highlight { get; set; }
```

### उदाहरण

पाठ के लिए शैली बदलने का तरीका दिखाता है।

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document document = new Document(dataDir + "Aspose.one");

// एक विशेष RichText नोड प्राप्त करें
RichText richText = document.GetChildNodes<RichText>().First();

foreach (var run in richText.TextRuns)
{
    // फ़ॉन्ट रंग सेट करें
    run.Style.FontColor = Color.Yellow;

    // हाइलाइट रंग सेट करें
    run.Style.Highlight = Color.Blue;

    // फ़ॉन्ट आकार सेट करें
    run.Style.FontSize = 20;
}
```

दिखाता है कि विभिन्न शैलियों के साथ पाठ वाली तालिका कैसे बनाई जाती है।

```csharp
string dataDir = RunExamples.GetDataDir_Text();

var headerText = new RichText() { ParagraphStyle = new ParagraphStyle() { FontSize = 18, IsBold = true }, Alignment = HorizontalAlignment.Center }
                    .Append("Super contest for suppliers.");

var page = new Page();
var outline = page.AppendChildLast(new Outline() { HorizontalOffset = 50 });
outline.AppendChildLast(new OutlineElement()).AppendChildLast(headerText);

// सार पाठ तालिका से पहले
var bodyTextHeader = outline.AppendChildLast(new OutlineElement()).AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default });
bodyTextHeader.Append("This is the final ranking of proposals got from our suppliers.");

var ranking = outline.AppendChildLast(new OutlineElement()).AppendChildLast(new Table());
var headerRow = ranking.AppendChildFirst(new TableRow());

var headerStyle = ParagraphStyle.Default;
headerStyle.IsBold = true;

// चलिए कॉलम का एक सेट और एक हेडर पंक्ति जोड़ते हैं
var backGroundColor = Color.LightGray;
foreach (var header in new[] { "Supplier", "Contacts", "Score A", "Score B", "Score C", "Final score", "Attached materials", "Comments" })
{
    ranking.Columns.Add(new TableColumn());
    headerRow.AppendChildLast(new TableCell() { BackgroundColor = backGroundColor })
             .AppendChildLast(new OutlineElement())
             .AppendChildLast(new RichText() { ParagraphStyle = headerStyle })
                .Append(header);
}

// चलो 5 खाली पंक्तियाँ। पंक्तियों में पृष्ठभूमि का रंग बदल रहा है
for (int i = 0; i < 5; i++)
{
    backGroundColor = backGroundColor.IsEmpty ? Color.LightGray : Color.Empty;

    var row = ranking.AppendChildLast(new TableRow());
    for (int j = 0; j < ranking.Columns.Count(); j++)
    {
        row.AppendChildLast(new TableCell() { BackgroundColor = backGroundColor })
           .AppendChildLast(new OutlineElement())
           .AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default });
    }
}

// चलिए 'संपर्क' कॉलम में सामग्री के लिए कुछ टेम्पलेट जोड़ते हैं
foreach (var row in ranking.Skip(1))
{
    var contactsCell = row.ElementAt(1);
    contactsCell.AppendChildLast(new OutlineElement())
                .AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default })
                    .Append("Web: ").Append("link", new TextStyle() { HyperlinkAddress = "www.link.com", IsHyperlink = true });
    contactsCell.AppendChildLast(new OutlineElement())
                .AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default })
                    .Append("E-mail: ").Append("mail", new TextStyle() { HyperlinkAddress = "mailto:hi@link.com", IsHyperlink = true });
}

var d = new Document();
d.AppendChildLast(page);
d.Save(Path.Combine(dataDir, "ComposeTable_out.one"));
```

### यह सभी देखें

* class [Style](../)
* नाम स्थान [Aspose.Note](../../style/)
* सभा [Aspose.Note](../../../)


