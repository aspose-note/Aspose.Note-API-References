---
title: PrintOptions.PageSplittingAlgorithm
second_title: Aspose.Note .NET API संदर्भ के लिए
description: PrintOptions संपत्त. पृष्ठ वभजन के लए उपयग कए जने वले एल्गरथ्म क प्रप्त य सेट करत है
type: docs
weight: 30
url: /hi/net/aspose.note.saving/printoptions/pagesplittingalgorithm/
---
## PrintOptions.PageSplittingAlgorithm property

पृष्ठ विभाजन के लिए उपयोग किए जाने वाले एल्गोरिथ्म को प्राप्त या सेट करता है।

```csharp
public PageSplittingAlgorithm PageSplittingAlgorithm { get; set; }
```

### संपत्ति मूल्य

द`PageSplittingAlgorithm` .

### उदाहरण

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

### यह सभी देखें

* class [PageSplittingAlgorithm](../../pagesplittingalgorithm/)
* class [PrintOptions](../)
* नाम स्थान [Aspose.Note.Saving](../../printoptions/)
* सभा [Aspose.Note](../../../)


