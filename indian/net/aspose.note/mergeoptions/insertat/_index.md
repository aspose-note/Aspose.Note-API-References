---
title: MergeOptions.InsertAt
second_title: Aspose.Note .NET API संदर्भ के लिए
description: MergeOptions संपत्त. उस स्थन क प्रप्त य सेट करत है जहं आयतत पृष्ठ डले जएंगे
type: docs
weight: 40
url: /hi/net/aspose.note/mergeoptions/insertat/
---
## MergeOptions.InsertAt property

उस स्थान को प्राप्त या सेट करता है जहां आयातित पृष्ठ डाले जाएंगे।

```csharp
public int InsertAt { get; set; }
```

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentOutOfRangeException |  |

### टिप्पणियों

यदि मान लक्ष्य दस्तावेज़ में पृष्ठों की संख्या से अधिक है तो आयातित पृष्ठ दस्तावेज़ के अंत में जोड़े जाते हैं।

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


