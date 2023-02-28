---
title: Document.Import
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Document तरक. प्रदन कए गए पडएफ दस्तवेज़ से पृष्ठं क एक सेट आयत करत है
type: docs
weight: 110
url: /hi/net/aspose.note/document/import/
---
## Import(Stream, PdfImportOptions, MergeOptions) {#import}

प्रदान किए गए पीडीएफ दस्तावेज़ से पृष्ठों का एक सेट आयात करता है।

```csharp
public Document Import(Stream stream, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| stream | Stream | पीडीएफ दस्तावेज़ के साथ एक स्ट्रीम। |
| importOptions | PdfImportOptions | पीडीएफ दस्तावेज़ से पृष्ठों को आयात करने के विकल्पों को निर्दिष्ट करता है। |
| mergeOptions | MergeOptions | प्रदान किए गए पृष्ठों को मर्ज करने के विकल्पों को निर्दिष्ट करता है. |

### प्रतिलाभ की मात्रा

दस्तावेज़ का संदर्भ देता है.

### यह सभी देखें

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* नाम स्थान [Aspose.Note](../../document/)
* सभा [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions, MergeOptions) {#import_1}

प्रदान किए गए पीडीएफ दस्तावेज़ से पृष्ठों का एक सेट आयात करता है।

```csharp
public Document Import(string file, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| file | String | PDF दस्तावेज़ वाली एक फ़ाइल. |
| importOptions | PdfImportOptions | पीडीएफ दस्तावेज़ से पृष्ठों को आयात करने के विकल्पों को निर्दिष्ट करता है। |
| mergeOptions | MergeOptions | प्रदान किए गए पृष्ठों को मर्ज करने के विकल्पों को निर्दिष्ट करता है. |

### प्रतिलाभ की मात्रा

दस्तावेज़ का संदर्भ देता है.

### उदाहरण

दिखाता है कि पीडीएफ दस्तावेज़ों के एक सेट से पेज दर पेज सभी पेजों को कैसे आयात किया जाए।

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

d.Import(Path.Combine(dataDir, "sampleText.pdf"))
 .Import(Path.Combine(dataDir, "sampleImage.pdf"))
 .Import(Path.Combine(dataDir, "sampleTable.pdf"));

d.Save(Path.Combine(dataDir, "sample_SimpleMerge.one"));
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

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* नाम स्थान [Aspose.Note](../../document/)
* सभा [Aspose.Note](../../../)


