---
title: Class NotebookSaveOptions
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.Saving.NotebookSaveOptions कक्ष. एक सर आधर वर्ग ज कस वशेष प्ररूप के लए नटबुक बचत वकल्पं क प्रतनधत्व करत है
type: docs
weight: 790
url: /hi/net/aspose.note.saving/notebooksaveoptions/
---
## NotebookSaveOptions class

एक सार आधार वर्ग जो किसी विशेष प्रारूप के लिए नोटबुक बचत विकल्पों का प्रतिनिधित्व करता है।

```csharp
public abstract class NotebookSaveOptions
```

## गुण

| नाम | विवरण |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | एक मान प्राप्त या सेट करता है जो इंगित करता है कि क्या बच्चों के दस्तावेज़ को स्पष्ट रूप से सहेजा जाना चाहिए। |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | एक मान प्राप्त या सेट करता है जो इंगित करता है कि क्या नोटबुक चिल्ड्रन पदानुक्रम को चपटा करके सहेजा गया है। |
| abstract [SaveFormat](../../aspose.note.saving/notebooksaveoptions/saveformat/) { get; } | उस प्रारूप को प्राप्त करता है जिसमें नोटबुक सहेजी जाती है। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| abstract [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions/getdocumentsaveoptions/)() | सभी नोटबुक के चाइल्ड दस्तावेज़ों के लिए सहेजें विकल्प प्राप्त करता है. |

### उदाहरण

चपटा नोटबुक को पीडीएफ प्रारूप में सहेजने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_NoteBook();

// एक OneNote नोटबुक लोड करें
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// नोटबुक को सेव करें
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

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

छवि के रूप में चपटी नोटबुक को सहेजने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_NoteBook();

// एक OneNote नोटबुक लोड करें
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// नोटबुक को सेव करें
notebook.Save(dataDir, notebookSaveOptions);
```

### यह सभी देखें

* नाम स्थान [Aspose.Note.Saving](../../aspose.note.saving/)
* सभा [Aspose.Note](../../)


