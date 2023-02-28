---
title: Class NotebookPdfSaveOptions
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.Saving.NotebookPdfSaveOptions कक्ष. नटबुक पृष्ठं क PDF में प्रस्तुत करते समय अतरक्त वकल्प नर्दष्ट करने क अनुमत देत है
type: docs
weight: 780
url: /hi/net/aspose.note.saving/notebookpdfsaveoptions/
---
## NotebookPdfSaveOptions class

नोटबुक पृष्ठों को PDF में प्रस्तुत करते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।

```csharp
public class NotebookPdfSaveOptions : NotebookSaveOptions<PdfSaveOptions>
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [NotebookPdfSaveOptions](notebookpdfsaveoptions/)() | डिफ़ॉल्ट कंस्ट्रक्टर। |

## गुण

| नाम | विवरण |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | एक मान प्राप्त या सेट करता है जो इंगित करता है कि क्या बच्चों के दस्तावेज़ को स्पष्ट रूप से सहेजा जाना चाहिए। |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } |  |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | एक मान प्राप्त या सेट करता है जो इंगित करता है कि क्या नोटबुक चिल्ड्रन पदानुक्रम को चपटा करके सहेजा गया है। |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } |  |

## तरीकों

| नाम | विवरण |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() |  |

### उदाहरण

दिखाता है कि निर्दिष्ट विकल्पों के साथ नोटबुक को पीडीएफ प्रारूप में कैसे सहेजा जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_NoteBook();

// एक OneNote नोटबुक लोड करें
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookPdfSaveOptions();

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

dataDir = dataDir + "ConvertToPDF_out.pdf";

// नोटबुक को सेव करें
notebook.Save(dataDir, notebookSaveOptions);
```

### यह सभी देखें

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../notebooksaveoptions-1/)
* class [PdfSaveOptions](../pdfsaveoptions/)
* नाम स्थान [Aspose.Note.Saving](../../aspose.note.saving/)
* सभा [Aspose.Note](../../)


