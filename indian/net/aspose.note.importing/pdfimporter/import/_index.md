---
title: PdfImporter.Import
second_title: Aspose.Note .NET API संदर्भ के लिए
description: PdfImporter तरक. प्रदन क गई स्ट्रम से PDF दस्तवेज़ क समग्र आयत करत है.
type: docs
weight: 10
url: /hi/net/aspose.note.importing/pdfimporter/import/
---
## Import(Stream, PdfImportOptions) {#import}

प्रदान की गई स्ट्रीम से PDF दस्तावेज़ की सामग्री आयात करता है.

```csharp
public static List<Page> Import(Stream stream, PdfImportOptions options = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| stream | Stream | स्ट्रीम. |
| options | PdfImportOptions | विकल्प। |

### प्रतिलाभ की मात्रा

द[`PdfImporter`](../) .

### यह सभी देखें

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* नाम स्थान [Aspose.Note.Importing](../../pdfimporter/)
* सभा [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions) {#import_1}

एक निर्दिष्ट फ़ाइल से पीडीएफ दस्तावेज़ की सामग्री आयात करता है।

```csharp
public static List<Page> Import(string file, PdfImportOptions options = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| file | String | पीडीएफ फाइल। |
| options | PdfImportOptions | विकल्प। |

### प्रतिलाभ की मात्रा

द[`PdfImporter`](../) .

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

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* नाम स्थान [Aspose.Note.Importing](../../pdfimporter/)
* सभा [Aspose.Note](../../../)


