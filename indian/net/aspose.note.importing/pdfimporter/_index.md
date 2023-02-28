---
title: Class PdfImporter
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.Importing.PdfImporter कक्ष. पडएफ प्ररूप में दस्तवेजं से समग्र आयत करने के लए एपआई प्रदन करने वल वर्ग एपआई नर्दष्ट वकल्पं क उपयग करके फ़इल य स्ट्रम में स्थत पडएफ दस्तवेज़ से आयत करने क अनुमत देत है आयत वकल्प क उपयग करके परत कय जत हैPdfImportOptions .
type: docs
weight: 270
url: /hi/net/aspose.note.importing/pdfimporter/
---
## PdfImporter class

पीडीएफ प्रारूप में दस्तावेजों से सामग्री आयात करने के लिए एपीआई प्रदान करने वाला वर्ग। एपीआई निर्दिष्ट विकल्पों का उपयोग करके फ़ाइल या स्ट्रीम में स्थित पीडीएफ दस्तावेज़ से आयात करने की अनुमति देता है। आयात विकल्प का उपयोग करके पारित किया जाता है[`PdfImportOptions`](../pdfimportoptions/) .

```csharp
public static class PdfImporter
```

## तरीकों

| नाम | विवरण |
| --- | --- |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import)(Stream, PdfImportOptions) | प्रदान की गई स्ट्रीम से PDF दस्तावेज़ की सामग्री आयात करता है. |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import_1)(string, PdfImportOptions) | एक निर्दिष्ट फ़ाइल से पीडीएफ दस्तावेज़ की सामग्री आयात करता है। |

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

* नाम स्थान [Aspose.Note.Importing](../../aspose.note.importing/)
* सभा [Aspose.Note](../../)


