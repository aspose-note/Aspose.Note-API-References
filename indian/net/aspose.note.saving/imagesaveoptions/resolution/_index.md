---
title: ImageSaveOptions.Resolution
second_title: Aspose.Note .NET API संदर्भ के लिए
description: ImageSaveOptions संपत्त. उत्पन्न छवयं के लए डट्स प्रत इंच में रज़ल्यूशन प्रप्त य सेट करत है
type: docs
weight: 50
url: /hi/net/aspose.note.saving/imagesaveoptions/resolution/
---
## ImageSaveOptions.Resolution property

उत्पन्न छवियों के लिए डॉट्स प्रति इंच में रिज़ॉल्यूशन प्राप्त या सेट करता है।

```csharp
public float Resolution { get; set; }
```

### टिप्पणियों

डिफ़ॉल्ट मान 96. है

### उदाहरण

दस्तावेज़ को छवि के रूप में सहेजते समय छवि रिज़ॉल्यूशन सेट करने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// दस्तावेज़ को सहेजें।
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

निर्दिष्ट विकल्पों के साथ नोटबुक को छवि के रूप में सहेजने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_NoteBook();

// एक OneNote नोटबुक लोड करें
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

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

* class [ImageSaveOptions](../)
* नाम स्थान [Aspose.Note.Saving](../../imagesaveoptions/)
* सभा [Aspose.Note](../../../)


