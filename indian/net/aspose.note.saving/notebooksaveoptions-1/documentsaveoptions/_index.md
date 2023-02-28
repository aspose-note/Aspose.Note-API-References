---
title: NotebookSaveOptions1.DocumentSaveOptions
second_title: Aspose.Note .NET API संदर्भ के लिए
description: NotebookSaveOptions संपत्त. सभ नटबुक के चइल्ड दस्तवेज़ं के लए सहेजें वकल्प प्रप्त करत है य सेट करत है.
type: docs
weight: 10
url: /hi/net/aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt;.DocumentSaveOptions property

सभी नोटबुक के चाइल्ड दस्तावेज़ों के लिए सहेजें विकल्प प्राप्त करता है या सेट करता है.

```csharp
public TDocumentSaveOptions DocumentSaveOptions { get; }
```

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

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../)
* नाम स्थान [Aspose.Note.Saving](../../notebooksaveoptions-1/)
* सभा [Aspose.Note](../../../)


