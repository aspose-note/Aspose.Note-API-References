---
title: MergeOptions.PageSpacing
second_title: Aspose.Note .NET API संदर्भ के लिए
description: MergeOptions संपत्त. एक पृष्ठ के रूप में आयत कए जने पर पृष्ठं के बच रक्त प्रप्त य सेट करत है
type: docs
weight: 50
url: /hi/net/aspose.note/mergeoptions/pagespacing/
---
## MergeOptions.PageSpacing property

एक पृष्ठ के रूप में आयात किए जाने पर पृष्ठों के बीच रिक्ति प्राप्त या सेट करता है।

```csharp
public float PageSpacing { get; set; }
```

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

* class [MergeOptions](../)
* नाम स्थान [Aspose.Note](../../mergeoptions/)
* सभा [Aspose.Note](../../../)


