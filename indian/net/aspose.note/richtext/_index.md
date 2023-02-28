---
title: Class RichText
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.RichText कक्ष. एक समृद्ध पठ क प्रतनधत्व करत है
type: docs
weight: 530
url: /hi/net/aspose.note/richtext/
---
## RichText class

एक समृद्ध पाठ का प्रतिनिधित्व करता है।

```csharp
public sealed class RichText : Node, IEnumerable<char>, IOutlineElementChildNode, ITaggable
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [RichText](richtext/#constructor)() | का एक नया उदाहरण प्रारंभ करता है`RichText` वर्ग. |

## गुण

| नाम | विवरण |
| --- | --- |
| [Alignment](../../aspose.note/richtext/alignment/) { get; set; } | संरेखण प्राप्त करता है या सेट करता है। |
| [Document](../../aspose.note/node/document/) { get; } | नोड का दस्तावेज़ प्राप्त करता है। |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | एक मान प्राप्त करता है जो इंगित करता है कि यह नोड समग्र है या नहीं। यदि सही है तो नोड में चाइल्ड नोड हो सकते हैं. |
| [LastModifiedTime](../../aspose.note/richtext/lastmodifiedtime/) { get; set; } | अंतिम संशोधित समय प्राप्त या सेट करता है। |
| [Length](../../aspose.note/richtext/length/) { get; } | पाठ की लंबाई प्राप्त करता है। |
| [LineSpacing](../../aspose.note/richtext/linespacing/) { get; set; } | लाइन स्पेसिंग प्राप्त या सेट करता है। |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | उसी नोड ट्री स्तर पर अगला नोड प्राप्त करता है। |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | नोड प्रकार प्राप्त करता है। |
| [ParagraphStyle](../../aspose.note/richtext/paragraphstyle/) { get; set; } | पैराग्राफ़ शैली को प्राप्त या सेट करता है।Styles संग्रह या तो यह ऑब्जेक्ट आवश्यक सेटिंग निर्दिष्ट नहीं करता है. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | मूल नोड प्राप्त करता है। |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | पिछले नोड को उसी नोड ट्री स्तर पर प्राप्त करता है। |
| [SpaceAfter](../../aspose.note/richtext/spaceafter/) { get; set; } | के बाद न्यूनतम स्थान प्राप्त या सेट करता है। |
| [SpaceBefore](../../aspose.note/richtext/spacebefore/) { get; set; } | पहले स्थान की न्यूनतम मात्रा प्राप्त या सेट करता है। |
| [Tags](../../aspose.note/richtext/tags/) { get; } | अनुच्छेद के सभी टैग की सूची प्राप्त करता है। |
| [Text](../../aspose.note/richtext/text/) { get; set; } | टेक्स्ट प्राप्त या सेट करता है। स्ट्रिंग में मान 10 (लाइन फ़ीड) का कोई वर्ण नहीं होना चाहिए . |
| [TextRuns](../../aspose.note/richtext/textruns/) { get; } | टेक्स्ट रन का संग्रह प्राप्त करता है। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| override [Accept](../../aspose.note/richtext/accept/)(DocumentVisitor) | नोड के आगंतुक को स्वीकार करता है। |
| [Append](../../aspose.note/richtext/append/#append)(string) | अंतिम पाठ श्रेणी में एक स्ट्रिंग जोड़ता है। |
| [Append](../../aspose.note/richtext/append/#append_1)(string, TextStyle) | अंत में एक स्ट्रिंग जोड़ता है। |
| [AppendFront](../../aspose.note/richtext/appendfront/#appendfront)(string) | पहली पाठ श्रेणी के सामने एक स्ट्रिंग जोड़ता है। |
| [AppendFront](../../aspose.note/richtext/appendfront/#appendfront_1)(string, TextStyle) | सामने एक स्ट्रिंग जोड़ता है। |
| [Clear](../../aspose.note/richtext/clear/)() | इस उदाहरण की सामग्री साफ़ करता है। |
| [GetEnumerator](../../aspose.note/richtext/getenumerator/)() | एन्यूमरेटर लौटाता है जो इस RichText ऑब्जेक्ट के वर्णों के माध्यम से पुनरावृति करता है। |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof)(char) | इस स्ट्रिंग में निर्दिष्ट यूनिकोड वर्ण की पहली घटना का शून्य-आधारित सूचकांक लौटाता है। |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_3)(string) | इस उदाहरण में निर्दिष्ट स्ट्रिंग की पहली घटना का शून्य-आधारित सूचकांक लौटाता है। |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_1)(char, int) | इस स्ट्रिंग में निर्दिष्ट यूनिकोड वर्ण की पहली घटना का शून्य-आधारित सूचकांक लौटाता है। खोज एक निर्दिष्ट वर्ण स्थिति पर शुरू होती है। |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_4)(string, int) | इस उदाहरण में निर्दिष्ट स्ट्रिंग की पहली घटना का शून्य-आधारित सूचकांक लौटाता है। खोज एक निर्दिष्ट वर्ण स्थिति पर शुरू होती है। |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_8)(string, StringComparison) | वर्तमान उदाहरण में निर्दिष्ट स्ट्रिंग की पहली घटना का शून्य-आधारित सूचकांक लौटाता है। एक पैरामीटर निर्दिष्ट स्ट्रिंग के लिए उपयोग करने के लिए खोज के प्रकार को निर्दिष्ट करता है। |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_2)(char, int, int) | इस उदाहरण में निर्दिष्ट वर्ण की पहली घटना का शून्य-आधारित सूचकांक लौटाता है। खोज एक निर्दिष्ट वर्ण स्थिति से शुरू होती है और एक निर्दिष्ट संख्या में वर्ण स्थिति की जांच करती है। |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_5)(string, int, int) | इस उदाहरण में निर्दिष्ट स्ट्रिंग की पहली घटना का शून्य-आधारित सूचकांक लौटाता है। खोज एक निर्दिष्ट वर्ण स्थिति से शुरू होती है और एक निर्दिष्ट संख्या में वर्ण स्थिति की जांच करती है। |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_7)(string, int, StringComparison) | वर्तमान उदाहरण में निर्दिष्ट स्ट्रिंग की पहली घटना का शून्य-आधारित सूचकांक लौटाता है। पैरामीटर वर्तमान स्ट्रिंग में प्रारंभिक खोज स्थिति और निर्दिष्ट स्ट्रिंग के लिए उपयोग करने के लिए खोज के प्रकार को निर्दिष्ट करते हैं। |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_6)(string, int, int, StringComparison) | वर्तमान उदाहरण में निर्दिष्ट स्ट्रिंग की पहली घटना का शून्य-आधारित सूचकांक लौटाता है। |
| [Insert](../../aspose.note/richtext/insert/#insert)(int, string) | इस उदाहरण में निर्दिष्ट इंडेक्स स्थिति पर एक निर्दिष्ट स्ट्रिंग सम्मिलित करता है। |
| [Insert](../../aspose.note/richtext/insert/#insert_1)(int, string, TextStyle) | इस उदाहरण में निर्दिष्ट इंडेक्स स्थिति पर निर्दिष्ट शैली के साथ एक निर्दिष्ट स्ट्रिंग सम्मिलित करता है। |
| [Remove](../../aspose.note/richtext/remove/#remove)(int) | वर्तमान उदाहरण में सभी वर्णों को हटाता है, एक निर्दिष्ट स्थान से शुरू होकर अंतिम स्थिति तक जारी रहता है। |
| [Remove](../../aspose.note/richtext/remove/#remove_1)(int, int) | निर्दिष्ट स्थान से शुरू होने वाले वर्तमान उदाहरण में वर्णों की निर्दिष्ट संख्या को हटाता है। |
| [Replace](../../aspose.note/richtext/replace/#replace)(char, char) | इस उदाहरण में एक निर्दिष्ट यूनिकोड वर्ण की सभी घटनाओं को दूसरे निर्दिष्ट यूनिकोड वर्ण के साथ बदल देता है। |
| [Replace](../../aspose.note/richtext/replace/#replace_1)(string, string) | वर्तमान उदाहरण में निर्दिष्ट स्ट्रिंग की सभी घटनाओं को अन्य निर्दिष्ट स्ट्रिंग के साथ बदलता है। |
| [Replace](../../aspose.note/richtext/replace/#replace_2)(string, string, TextStyle) | वर्तमान उदाहरण में निर्दिष्ट स्ट्रिंग की सभी घटनाओं को निर्दिष्ट शैली में अन्य निर्दिष्ट स्ट्रिंग के साथ बदलता है। |
| [Trim](../../aspose.note/richtext/trim/#trim)() | सभी प्रमुख और अनुगामी व्हाइट-स्पेस वर्णों को हटाता है। |
| [Trim](../../aspose.note/richtext/trim/#trim_1)(char) | एक चरित्र के सभी प्रमुख और अनुगामी उदाहरणों को हटाता है। |
| [Trim](../../aspose.note/richtext/trim/#trim_2)(params char[]) | एक सरणी में निर्दिष्ट वर्णों के एक सेट की सभी प्रमुख और अनुगामी घटनाओं को हटाता है। |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend)() | सभी अनुगामी श्वेत-स्थान वर्णों को हटाता है। |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend_1)(char) | एक वर्ण की सभी अनुगामी घटनाओं को हटाता है। |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend_2)(params char[]) | एक सरणी में निर्दिष्ट वर्णों के एक समूह की सभी अनुगामी घटनाओं को हटाता है। |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart)() | सभी प्रमुख व्हाइट-स्पेस वर्णों को हटाता है। |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart_1)(char) | निर्दिष्ट वर्ण की सभी प्रमुख घटनाओं को हटाता है। |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart_2)(params char[]) | एक सरणी में निर्दिष्ट वर्णों के एक सेट की सभी प्रमुख घटनाओं को हटा देता है। |

### उदाहरण

दस्तावेज़ से सभी पाठ प्राप्त करने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Text();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

// पाठ पुनर्प्राप्त करें
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// आउटपुट स्क्रीन पर टेक्स्ट प्रिंट करें
Console.WriteLine(text);
```

दिखाता है कि पृष्ठ से सभी पाठ कैसे प्राप्त करें।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Text();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

// पेज नोड्स की सूची प्राप्त करें
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // पाठ पुनर्प्राप्त करें
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // आउटपुट स्क्रीन पर टेक्स्ट प्रिंट करें
    Console.WriteLine(text);
}
```

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

दिखाता है कि प्रत्येक तालिका की पंक्ति से टेक्स्ट कैसे प्राप्त करें।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Tables();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document document = new Document(dataDir + "Sample1.one");

// टेबल नोड्स की सूची प्राप्त करें
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // तालिका पंक्तियों के माध्यम से पुनरावृति करें
    foreach (TableRow row in table)
    {
        // पाठ पुनर्प्राप्त करें
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // आउटपुट स्क्रीन पर टेक्स्ट प्रिंट करें
        Console.WriteLine(text);
    }
}
```

तालिका से टेक्स्ट प्राप्त करने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Tables();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document document = new Document(dataDir + "Sample1.one");

// टेबल नोड्स की सूची प्राप्त करें
IList<Table> nodes = document.GetChildNodes<Table>();

// टेबल काउंट सेट करें
int tblCount = 0;

foreach (Table table in nodes)
{
    tblCount++;
    Console.WriteLine("table # " + tblCount);

    // पाठ पुनर्प्राप्त करें
    string text = string.Join(Environment.NewLine, table.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

    // आउटपुट स्क्रीन पर टेक्स्ट प्रिंट करें
    Console.WriteLine(text);
}
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

दिखाता है कि पृष्ठ के लिए शीर्षक कैसे सेट करें।

```csharp
string dataDir = RunExamples.GetDataDir_Text();
string outputPath = dataDir + "CreateTitleMsStyle_out.one";

var doc = new Document();
var page = new Page(doc);

page.Title = new Title(doc)
{
    TitleText = new RichText(doc)
    {
        Text = "Title text.",
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleDate = new RichText(doc)
    {
        Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture),
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleTime = new RichText(doc)
    {
        Text = "12:34",
        ParagraphStyle = ParagraphStyle.Default
    }
};

doc.AppendChildLast(page);

doc.Save(outputPath);
```

टेक्स्ट के लिए अशुद्धि जाँच भाषा सेट करें।

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = ParagraphStyle.Default };
text.Append("United States", new TextStyle() { Language = CultureInfo.GetCultureInfo("en-US") })
    .Append(" Germany", new TextStyle() { Language = CultureInfo.GetCultureInfo("de-DE") })
    .Append(" China", new TextStyle() { Language = CultureInfo.GetCultureInfo("zh-CN") });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetProofingLanguageForText.one"));
```

दिखाता है कि कैसे सभी पृष्ठों से गुजरना है और पाठ में एक प्रतिस्थापन करना है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

// सभी रिचटेक्स्ट नोड्स प्राप्त करें
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // किसी आकृति का पाठ बदलें
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

// किसी भी समर्थित फ़ाइल स्वरूप में सहेजें
oneFile.Save(dataDir, SaveFormat.Pdf);
```

अनुच्छेद शैली का उपयोग करके पाठ प्रारूप में हेरफेर करें।

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = new ParagraphStyle() { FontName = "Courier New", FontSize = 20 } }
                .Append($"DefaultParagraphFontAndSize{Environment.NewLine}")
                .Append($"OnlyDefaultParagraphFont{Environment.NewLine}", new TextStyle() { FontSize = 14 })
                .Append("OnlyDefaultParagraphFontSize", new TextStyle() { FontName = "Verdana" });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetDefaultParagraphStyle.one"));
```

टेबल के सेल से टेक्स्ट प्राप्त करने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Tables();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document document = new Document(dataDir + "Sample1.one");

// टेबल नोड्स की सूची प्राप्त करें
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // तालिका पंक्तियों के माध्यम से पुनरावृति करें
    foreach (TableRow row in table)
    {
        // टेबलसेल नोड्स की सूची प्राप्त करें
        // तालिका कक्षों के माध्यम से पुनरावृति करें
        foreach (TableCell cell in row)
        {
            // पाठ पुनर्प्राप्त करें
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // आउटपुट स्क्रीन पर टेक्स्ट प्रिंट करें
            Console.WriteLine(text);
        }
    }
}
```

दिखाता है कि पेज के टेक्स्ट को कैसे पास करना है और कैसे रिप्लेसमेंट करना है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// सभी रिचटेक्स्ट नोड्स प्राप्त करें
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // किसी आकृति का पाठ बदलें
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// किसी भी समर्थित फ़ाइल स्वरूप में सहेजें
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

दिखाता है कि एक दस्तावेज़ कैसे बनाया जाए और इसे डिफ़ॉल्ट विकल्पों का उपयोग करके HTML प्रारूप में कैसे सहेजा जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// OneNote दस्तावेज़ को प्रारंभ करें
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

// दस्तावेज़ में सभी पाठ के लिए डिफ़ॉल्ट शैली।
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// HTML फॉर्मेट में सेव करें
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

टैग के साथ नया पैराग्राफ जोड़ने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Tags();

// दस्तावेज़ वर्ग का एक ऑब्जेक्ट बनाएँ
Document doc = new Document();

// पेज क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// आउटलाइन क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Outline outline = new Outline(doc);

// आउटलाइन एलिमेंट क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
OutlineElement outlineElem = new OutlineElement(doc);
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
RichText text = new RichText(doc) { Text = "OneNote text.", ParagraphStyle = textStyle };
text.Tags.Add(NoteTag.CreateYellowStar());

// टेक्स्ट नोड जोड़ें
outlineElem.AppendChildLast(text);

// रूपरेखा तत्व नोड जोड़ें
outline.AppendChildLast(outlineElem);

// आउटलाइन नोड जोड़ें
page.AppendChildLast(outline);

// पेज नोड जोड़ें
doc.AppendChildLast(page);

// OneNote दस्तावेज़ सहेजें
dataDir = dataDir + "AddTextNodeWithTag_out.one";
doc.Save(dataDir);
```

दिखाता है कि दस्तावेज़ कैसे बनाया जाए और HTML प्रारूप में निर्दिष्ट पृष्ठों की श्रेणी में सहेजा जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// OneNote दस्तावेज़ को प्रारंभ करें
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// दस्तावेज़ में सभी पाठ के लिए डिफ़ॉल्ट शैली।
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// HTML फॉर्मेट में सेव करें
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

टैग के विवरण तक पहुंचने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Tags();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "TagFile.one");

// सभी रिचटेक्स्ट नोड्स प्राप्त करें
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// प्रत्येक नोड के माध्यम से दोहराएं
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // गुणों को पुनः प्राप्त करें
            Console.WriteLine($"    Completed Time: {noteTag.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTag.CreationTime}");
            Console.WriteLine($"    Font Color: {noteTag.FontColor}");
            Console.WriteLine($"    Status: {noteTag.Status}");
            Console.WriteLine($"    Label: {noteTag.Label}");
            Console.WriteLine($"    Icon: {noteTag.Icon}");
            Console.WriteLine($"    High Light: {noteTag.Highlight}");
        }
    }
}
```

पाठ के साथ दस्तावेज़ बनाने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ वर्ग का एक ऑब्जेक्ट बनाएँ
Document doc = new Document();

// पेज क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Page page = new Page(doc);

// आउटलाइन क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Outline outline = new Outline(doc);

// आउटलाइन एलिमेंट क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
OutlineElement outlineElem = new OutlineElement(doc);

// टेक्स्ट स्टाइल क्लास ऑब्जेक्ट प्रारंभ करें और स्वरूपण गुण सेट करें
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// RichText क्लास ऑब्जेक्ट को इनिशियलाइज़ करें और टेक्स्ट स्टाइल लागू करें
RichText text = new RichText(doc) { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// रिचटेक्स्ट नोड जोड़ें
outlineElem.AppendChildLast(text);

// आउटलाइन एलिमेंट नोड जोड़ें
outline.AppendChildLast(outlineElem);

// आउटलाइन नोड जोड़ें
page.AppendChildLast(outline);

// पेज नोड जोड़ें
doc.AppendChildLast(page);

// OneNote दस्तावेज़ सहेजें
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
doc.Save(dataDir);
```

दिखाता है कि चीनी क्रमांकन के साथ नई सूची कैसे सम्मिलित करें।

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// OneNote दस्तावेज़ को प्रारंभ करें
Aspose.Note.Document doc = new Aspose.Note.Document();

// OneNote पेज को इनिशियलाइज़ करें
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// टेक्स्ट स्टाइल सेटिंग लागू करें
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// एक ही रूपरेखा में संख्याएँ स्वतः बढ़ जाती हैं।
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

//---------------------------------------------------------------------
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

//---------------------------------------------------------------------
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

//---------------------------------------------------------------------
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// OneNote दस्तावेज़ सहेजें
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

दिखाता है कि नई बुलेटेड लिस कैसे डालें।

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// दस्तावेज़ वर्ग का एक ऑब्जेक्ट बनाएँ
Aspose.Note.Document doc = new Aspose.Note.Document();

// पेज क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// आउटलाइन क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Outline outline = new Outline(doc);

// टेक्स्ट स्टाइल क्लास ऑब्जेक्ट प्रारंभ करें और स्वरूपण गुण सेट करें
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// OutlineElement क्लास ऑब्जेक्ट को इनिशियलाइज़ करें और बुलेट्स अप्लाई करें
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// RichText क्लास ऑब्जेक्ट को इनिशियलाइज़ करें और टेक्स्ट स्टाइल लागू करें
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// रूपरेखा तत्व जोड़ें
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// आउटलाइन नोड जोड़ें
page.AppendChildLast(outline);
// पेज नोड जोड़ें
doc.AppendChildLast(page);

// OneNote दस्तावेज़ सहेजें
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

नंबरिंग के साथ नई सूची डालने का तरीका दिखाता है।

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// दस्तावेज़ वर्ग का एक ऑब्जेक्ट बनाएँ
Document doc = new Document();

// पेज क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// आउटलाइन क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Outline outline = new Outline(doc);

// टेक्स्ट स्टाइल क्लास ऑब्जेक्ट प्रारंभ करें और स्वरूपण गुण सेट करें
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// आउटलाइन एलिमेंट क्लास ऑब्जेक्ट्स को इनिशियलाइज़ करें और नंबरिंग लागू करें
// एक ही रूपरेखा में संख्याएँ स्वतः बढ़ जाती हैं।
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// रूपरेखा तत्व जोड़ें
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// आउटलाइन नोड जोड़ें
page.AppendChildLast(outline);

// पेज नोड जोड़ें
doc.AppendChildLast(page);

// OneNote दस्तावेज़ सहेजें
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

दिखाता है कि साप्ताहिक बैठक के लिए एक खाका कैसे तैयार किया जाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Tags();

// दस्तावेज़ वर्ग का एक ऑब्जेक्ट बनाएँ
var headerStyle = new ParagraphStyle() { FontName = "Calibri", FontSize = 16 };
var bodyStyle = new ParagraphStyle() { FontName = "Calibri", FontSize = 12 };

var d = new Document();
bool restartFlag = true;
var outline = d.AppendChildLast(new Page()
                                    {
                                        Title = new Title() { TitleText = new RichText() { Text = $"Weekly meeting {DateTime.Today:d}", ParagraphStyle = ParagraphStyle.Default } }
                                    })
               .AppendChildLast(new Outline() { VerticalOffset = 30, HorizontalOffset = 30 });

outline.AppendChildLast(new OutlineElement())
       .AppendChildLast(new RichText() { Text = "Important", ParagraphStyle = headerStyle });
foreach (var e in new[] { "First", "Second", "Third" })
{
    outline.AppendChildLast(new OutlineElement() { NumberList = CreateListNumberingStyle(bodyStyle, restartFlag) })
           .AppendChildLast(new RichText() { Text = e, ParagraphStyle = bodyStyle });
    restartFlag = false;
}

outline.AppendChildLast(new OutlineElement())
       .AppendChildLast(new RichText() { Text = "TO DO", ParagraphStyle = headerStyle, SpaceBefore = 15 });
restartFlag = true;
foreach (var e in new[] { "First", "Second", "Third" })
{
    outline.AppendChildLast(new OutlineElement() { NumberList = CreateListNumberingStyle(bodyStyle, restartFlag) })
           .AppendChildLast(new RichText() { Text = e, ParagraphStyle = bodyStyle, Tags = { NoteCheckBox.CreateBlueCheckBox() } });
    restartFlag = false;
}

d.Save(Path.Combine(dataDir, "meetingNotes.one"));
```

दिखाता है कि हाइपरलिंक को टेक्स्ट से कैसे बाइंड किया जाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Tasks();

// दस्तावेज़ वर्ग का एक ऑब्जेक्ट बनाएँ
Document doc = new Document();

RichText titleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append("Title!");

Outline outline = new Outline()
                      {
                          MaxWidth = 200,
                          MaxHeight = 200,
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };

TextStyle textStyleRed = new TextStyle
                             {
                                 FontColor = Color.Red,
                                 FontName = "Arial",
                                 FontSize = 10,
                             };

TextStyle textStyleHyperlink = new TextStyle
                                   {
                                       IsHyperlink = true,
                                       HyperlinkAddress = "www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// रूपरेखा तत्व जोड़ें
outline.AppendChildLast(outlineElem);

// टाइटल क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Title title = new Title() { TitleText = titleText };

// पेज क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Page page = new Note.Page() { Title = title };

// आउटलाइन नोड जोड़ें
page.AppendChildLast(outline);

// पेज नोड जोड़ें
doc.AppendChildLast(page);

// OneNote दस्तावेज़ सहेजें
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

### यह सभी देखें

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [ITaggable](../itaggable/)
* नाम स्थान [Aspose.Note](../../aspose.note/)
* सभा [Aspose.Note](../../)


