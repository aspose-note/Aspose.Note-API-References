---
title: NotebookSaveOptions.Flatten
second_title: Aspose.Note .NET API संदर्भ के लिए
description: NotebookSaveOptions संपत्त. एक मन प्रप्त य सेट करत है ज इंगत करत है क क्य नटबुक चल्ड्रन पदनुक्रम क चपट करके सहेज गय है
type: docs
weight: 20
url: /hi/net/aspose.note.saving/notebooksaveoptions/flatten/
---
## NotebookSaveOptions.Flatten property

एक मान प्राप्त या सेट करता है जो इंगित करता है कि क्या नोटबुक चिल्ड्रन पदानुक्रम को चपटा करके सहेजा गया है।

```csharp
public bool Flatten { get; set; }
```

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

* class [NotebookSaveOptions](../)
* नाम स्थान [Aspose.Note.Saving](../../notebooksaveoptions/)
* सभा [Aspose.Note](../../../)


