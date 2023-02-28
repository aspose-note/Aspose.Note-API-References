---
title: Document.Merge
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Document तरक. पृष्ठं के एक सेट क दस्तवेज़ में मर्ज करत है
type: docs
weight: 120
url: /hi/net/aspose.note/document/merge/
---
## Document.Merge method

पृष्ठों के एक सेट को दस्तावेज़ में मर्ज करता है।

```csharp
public Document Merge(IEnumerable<Page> pages, MergeOptions mergeOptions = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pages | IEnumerable`1 | पृष्ठों का एक सेट। |
| mergeOptions | MergeOptions | प्रदान किए गए पृष्ठों को मर्ज करने के विकल्पों को निर्दिष्ट करता है. |

### प्रतिलाभ की मात्रा

दस्तावेज़ का संदर्भ देता है.

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

### यह सभी देखें

* class [Page](../../page/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* नाम स्थान [Aspose.Note](../../document/)
* सभा [Aspose.Note](../../../)


