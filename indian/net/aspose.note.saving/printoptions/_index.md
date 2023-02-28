---
title: Class PrintOptions
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.Saving.PrintOptions कक्ष. दस्तवेज़ प्रंट करने के लए उपयग कए जने वले वकल्प.
type: docs
weight: 860
url: /hi/net/aspose.note.saving/printoptions/
---
## PrintOptions class

दस्तावेज़ प्रिंट करने के लिए उपयोग किए जाने वाले विकल्प.

```csharp
public class PrintOptions
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [PrintOptions](printoptions/)() | डिफ़ॉल्ट कंस्ट्रक्टर। |

## गुण

| नाम | विवरण |
| --- | --- |
| [DocumentName](../../aspose.note.saving/printoptions/documentname/) { get; set; } | दस्तावेज़ को प्रिंट करते समय प्रदर्शित करने के लिए दस्तावेज़ का नाम प्राप्त करता है या सेट करता है (उदाहरण के लिए, प्रिंट स्थिति संवाद बॉक्स या प्रिंटर कतार में)। |
| [PageSplittingAlgorithm](../../aspose.note.saving/printoptions/pagesplittingalgorithm/) { get; set; } | पृष्ठ विभाजन के लिए उपयोग किए जाने वाले एल्गोरिथ्म को प्राप्त या सेट करता है। |
| [PrinterSettings](../../aspose.note.saving/printoptions/printersettings/) { get; set; } | प्रिंटर सेटिंग्स प्राप्त या सेट करता है। |
| [Resolution](../../aspose.note.saving/printoptions/resolution/) { get; set; } | उत्पन्न छवियों के लिए डॉट्स प्रति इंच में रिज़ॉल्यूशन प्राप्त या सेट करता है। |

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

* नाम स्थान [Aspose.Note.Saving](../../aspose.note.saving/)
* सभा [Aspose.Note](../../)


