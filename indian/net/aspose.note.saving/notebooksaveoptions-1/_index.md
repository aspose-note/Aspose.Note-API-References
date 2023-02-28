---
title: Class NotebookSaveOptionsTDocumentSaveOptions
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.Saving.NotebookSaveOptions1TDocumentSaveOptions कक्ष. एक सर आधर वर्ग ज कस वशेष प्ररूप के लए नटबुक बचत वकल्पं क प्रतनधत्व करत है और सभ दस्तवेज़ चइल्ड नड्स के लए समन्य बचत वकल्प प्रदन करत है
type: docs
weight: 800
url: /hi/net/aspose.note.saving/notebooksaveoptions-1/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt; class

एक सार आधार वर्ग जो किसी विशेष प्रारूप के लिए नोटबुक बचत विकल्पों का प्रतिनिधित्व करता है और सभी दस्तावेज़ चाइल्ड नोड्स के लिए सामान्य बचत विकल्प प्रदान करता है।

```csharp
public abstract class NotebookSaveOptions<TDocumentSaveOptions> : NotebookSaveOptions
    where TDocumentSaveOptions : SaveOptions
```

| पैरामीटर | विवरण |
| --- | --- |
| TDocumentSaveOptions | सभी नोटबुक के चाइल्ड दस्तावेज़ों के लिए सहेजें विकल्प. |

## गुण

| नाम | विवरण |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | एक मान प्राप्त या सेट करता है जो इंगित करता है कि क्या बच्चों के दस्तावेज़ को स्पष्ट रूप से सहेजा जाना चाहिए। |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } | सभी नोटबुक के चाइल्ड दस्तावेज़ों के लिए सहेजें विकल्प प्राप्त करता है या सेट करता है. |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | एक मान प्राप्त या सेट करता है जो इंगित करता है कि क्या नोटबुक चिल्ड्रन पदानुक्रम को चपटा करके सहेजा गया है। |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } | उस प्रारूप को प्राप्त करता है जिसमें नोटबुक सहेजी जाती है। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() | सभी नोटबुक के चाइल्ड दस्तावेज़ों के लिए सहेजें विकल्प प्राप्त करता है. |

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

* class [NotebookSaveOptions](../notebooksaveoptions/)
* class [SaveOptions](../saveoptions/)
* नाम स्थान [Aspose.Note.Saving](../../aspose.note.saving/)
* सभा [Aspose.Note](../../)


