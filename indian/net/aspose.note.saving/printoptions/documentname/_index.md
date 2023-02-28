---
title: PrintOptions.DocumentName
second_title: Aspose.Note .NET API संदर्भ के लिए
description: PrintOptions संपत्त. दस्तवेज़ क प्रंट करते समय प्रदर्शत करने के लए दस्तवेज़ क नम प्रप्त करत है य सेट करत है उदहरण के लए प्रंट स्थत संवद बक्स य प्रंटर कतर में
type: docs
weight: 20
url: /hi/net/aspose.note.saving/printoptions/documentname/
---
## PrintOptions.DocumentName property

दस्तावेज़ को प्रिंट करते समय प्रदर्शित करने के लिए दस्तावेज़ का नाम प्राप्त करता है या सेट करता है (उदाहरण के लिए, प्रिंट स्थिति संवाद बॉक्स या प्रिंटर कतार में)।

```csharp
public string DocumentName { get; set; }
```

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

* class [PrintOptions](../)
* नाम स्थान [Aspose.Note.Saving](../../printoptions/)
* सभा [Aspose.Note](../../../)


