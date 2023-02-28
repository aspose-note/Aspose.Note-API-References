---
title: Class MergeOptions
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.MergeOptions कक्ष. पृष्ठं के संग्रह क मर्ज करने के वकल्प
type: docs
weight: 340
url: /hi/net/aspose.note/mergeoptions/
---
## MergeOptions class

पृष्ठों के संग्रह को मर्ज करने के विकल्प।

```csharp
public class MergeOptions
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [MergeOptions](mergeoptions/)() | डिफ़ॉल्ट कंस्ट्रक्टर। |

## गुण

| नाम | विवरण |
| --- | --- |
| [ImportAsSinglePage](../../aspose.note/mergeoptions/importassinglepage/) { get; set; } | एक मान प्राप्त या सेट करता है जो इंगित करता है कि प्रदान किए गए पृष्ठों को एकल पृष्ठ के रूप में आयात करना है या नहीं। |
| [InsertAsChild](../../aspose.note/mergeoptions/insertaschild/) { get; set; } | एक मान प्राप्त या सेट करता है जो इंगित करता है कि सम्मिलित पृष्ठों को पिछले पृष्ठ के बच्चों के रूप में जोड़ा जाना चाहिए। |
| [InsertAt](../../aspose.note/mergeoptions/insertat/) { get; set; } | उस स्थान को प्राप्त या सेट करता है जहां आयातित पृष्ठ डाले जाएंगे। |
| [PageSpacing](../../aspose.note/mergeoptions/pagespacing/) { get; set; } | एक पृष्ठ के रूप में आयात किए जाने पर पृष्ठों के बीच रिक्ति प्राप्त या सेट करता है। |

### उदाहरण

दिखाता है कि प्रत्येक 5 पृष्ठों को एक एकल OneNote पृष्ठ पर समूहित करके PDF दस्तावेज़ से सभी पृष्ठों को कैसे आयात किया जाए।

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

var mergeOptions = new MergeOptions() { ImportAsSinglePage = true, PageSpacing = 100 };

IEnumerable<Page> pages = PdfImporter.Import(Path.Combine(dataDir, "SampleGrouping.pdf"));
while (pages.Any())
{
    d.Merge(pages.Take(5), mergeOptions);
    pages = pages.Skip(5);
}

d.Save(Path.Combine(dataDir, "sample_CustomMerge.one"));
```

शीर्ष स्तर के OneNote पृष्ठ के चिल्ड्रन के रूप में प्रत्येक PDF दस्तावेज़ से पृष्ठ सम्मिलित करते हुए PDF दस्तावेज़ों के सेट से सभी पृष्ठों को आयात करने का तरीका दिखाता है।

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

foreach (var file in new[] { "sampleText.pdf", "sampleImage.pdf", "sampleTable.pdf" })
{
    d.AppendChildLast(new Page()).Title = new Title() { TitleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append(file) };
    d.Import(Path.Combine(dataDir, file), new PdfImportOptions(), new MergeOptions() { InsertAt = int.MaxValue, InsertAsChild = true });
}

d.Save(Path.Combine(dataDir, "sample_StructuredMerge.one"));
```

प्रत्येक PDF दस्तावेज़ से एकल OneNote पृष्ठ में पृष्ठों को मर्ज करते समय PDF दस्तावेज़ों के सेट से सभी सामग्री को आयात करने का तरीका दिखाता है।

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

var importOptions = new PdfImportOptions();
var mergeOptions = new MergeOptions() { ImportAsSinglePage = true, PageSpacing = 100 };

d.Import(Path.Combine(dataDir, "sampleText.pdf"), importOptions, mergeOptions)
 .Import(Path.Combine(dataDir, "sampleImage.pdf"), importOptions, mergeOptions)
 .Import(Path.Combine(dataDir, "sampleTable.pdf"), importOptions, mergeOptions);

d.Save(Path.Combine(dataDir, "sample_SinglePageMerge.one"));
```

### यह सभी देखें

* नाम स्थान [Aspose.Note](../../aspose.note/)
* सभा [Aspose.Note](../../)


