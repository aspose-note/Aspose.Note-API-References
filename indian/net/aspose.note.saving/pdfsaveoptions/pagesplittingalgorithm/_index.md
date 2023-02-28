---
title: PdfSaveOptions.PageSplittingAlgorithm
second_title: Aspose.Note .NET API संदर्भ के लिए
description: PdfSaveOptions संपत्त. पृष्ठ वभजन के लए उपयग कए जने वले एल्गरथ्म क प्रप्त य सेट करत है
type: docs
weight: 50
url: /hi/net/aspose.note.saving/pdfsaveoptions/pagesplittingalgorithm/
---
## PdfSaveOptions.PageSplittingAlgorithm property

पृष्ठ विभाजन के लिए उपयोग किए जाने वाले एल्गोरिथ्म को प्राप्त या सेट करता है।

```csharp
public PageSplittingAlgorithm PageSplittingAlgorithm { get; set; }
```

### संपत्ति मूल्य

द`PageSplittingAlgorithm` .

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

जब लंबे OneNote पृष्ठ pdf स्वरूप में सहेजे जाते हैं, तो वे पृष्ठों में विभाजित हो जाते हैं. नमूना दिखाता है कि पृष्ठ के विरामों पर स्थित वस्तुओं के विभाजन तर्क को कैसे कॉन्फ़िगर किया जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// या
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

जब लंबे OneNote पृष्ठ pdf स्वरूप में सहेजे जाते हैं, तो वे पृष्ठों में विभाजित हो जाते हैं. उदाहरण दिखाता है कि पृष्ठ के विरामों पर स्थित वस्तुओं के विभाजन तर्क को कैसे कॉन्फ़िगर किया जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// या
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// या
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// या
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// या
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

### यह सभी देखें

* class [PageSplittingAlgorithm](../../pagesplittingalgorithm/)
* class [PdfSaveOptions](../)
* नाम स्थान [Aspose.Note.Saving](../../pdfsaveoptions/)
* सभा [Aspose.Note](../../../)


