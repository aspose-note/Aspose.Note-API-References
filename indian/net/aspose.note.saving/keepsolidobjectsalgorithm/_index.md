---
title: Class KeepSolidObjectsAlgorithm
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.Saving.KeepSolidObjectsAlgorithm कक्ष. पूरे ऑब्जेक्ट क अगले पेज पर शफ्ट कर देत है अगर यह मूल पेज में फट नहं हत है
type: docs
weight: 740
url: /hi/net/aspose.note.saving/keepsolidobjectsalgorithm/
---
## KeepSolidObjectsAlgorithm class

पूरे ऑब्जेक्ट को अगले पेज पर शिफ्ट कर देता है, अगर यह मूल पेज में फिट नहीं होता है।

```csharp
public class KeepSolidObjectsAlgorithm : PageSplittingAlgorithm
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [KeepSolidObjectsAlgorithm](keepsolidobjectsalgorithm/#constructor)() | का एक नया उदाहरण प्रारंभ करता है`KeepSolidObjectsAlgorithm` वर्ग क्लोन किए गए भाग की डिफ़ॉल्ट ऊंचाई सीमा का उपयोग कर रहा है। |
| [KeepSolidObjectsAlgorithm](keepsolidobjectsalgorithm/#constructor_1)(float) | का एक नया उदाहरण प्रारंभ करता है`KeepSolidObjectsAlgorithm` क्लोन किए गए भाग की विशिष्ट ऊंचाई सीमा का उपयोग करते हुए वर्ग. |

## गुण

| नाम | विवरण |
| --- | --- |
| [HeightLimitOfClonedPart](../../aspose.note.saving/keepsolidobjectsalgorithm/heightlimitofclonedpart/) { get; } | क्लोन किए गए भाग की ऊंचाई सीमा प्राप्त करता है। |

## खेत

| नाम | विवरण |
| --- | --- |
| const [DefaultHeightLimitOfClonedPart](../../aspose.note.saving/keepsolidobjectsalgorithm/defaultheightlimitofclonedpart/) | क्लोन किए गए भाग का डिफ़ॉल्ट अधिकतम आकार। |

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

निर्दिष्ट विकल्पों के साथ मानक विंडोज संवाद का उपयोग करके प्रिंटर को दस्तावेज़ भेजने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

var printerSettings = new PrinterSettings() { FromPage = 0, ToPage = 10 };
printerSettings.DefaultPageSettings.Landscape = true;
printerSettings.DefaultPageSettings.Margins = new System.Drawing.Printing.Margins(50, 50, 150, 50);

document.Print(new PrintOptions()
               {
                   PrinterSettings = printerSettings,
                   Resolution = 1200,
                   PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(),
                   DocumentName = "Test.one"
               });
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

* class [PageSplittingAlgorithm](../pagesplittingalgorithm/)
* नाम स्थान [Aspose.Note.Saving](../../aspose.note.saving/)
* सभा [Aspose.Note](../../)


