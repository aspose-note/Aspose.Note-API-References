---
title: MergeOptions.InsertAsChild
second_title: Aspose.Note .NET API संदर्भ के लिए
description: MergeOptions संपत्त. एक मन प्रप्त य सेट करत है ज इंगत करत है क सम्मलत पृष्ठं क पछले पृष्ठ के बच्चं के रूप में जड़ जन चहए
type: docs
weight: 30
url: /hi/net/aspose.note/mergeoptions/insertaschild/
---
## MergeOptions.InsertAsChild property

एक मान प्राप्त या सेट करता है जो इंगित करता है कि सम्मिलित पृष्ठों को पिछले पृष्ठ के बच्चों के रूप में जोड़ा जाना चाहिए।

```csharp
public bool InsertAsChild { get; set; }
```

### उदाहरण

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

### यह सभी देखें

* class [MergeOptions](../)
* नाम स्थान [Aspose.Note](../../mergeoptions/)
* सभा [Aspose.Note](../../../)


