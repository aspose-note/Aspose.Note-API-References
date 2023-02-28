---
title: Document.Print
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Document तरक. दस्तवेज़ क डफ़ल्ट प्रंटर क उपयग करके प्रंट करत है.
type: docs
weight: 130
url: /hi/net/aspose.note/document/print/
---
## Print() {#print}

दस्तावेज़ को डिफ़ॉल्ट प्रिंटर का उपयोग करके प्रिंट करता है.

```csharp
public void Print()
```

### उदाहरण

डिफ़ॉल्ट विकल्पों के साथ मानक विंडोज संवाद का उपयोग करके प्रिंटर को दस्तावेज़ भेजने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
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

### यह सभी देखें

* class [Document](../)
* नाम स्थान [Aspose.Note](../../document/)
* सभा [Aspose.Note](../../../)

---

## Print(PrintOptions) {#print_1}

दस्तावेज़ को डिफ़ॉल्ट प्रिंटर का उपयोग करके प्रिंट करता है.

```csharp
public void Print(PrintOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| options | PrintOptions | दस्तावेज़ प्रिंट करने के लिए उपयोग किए जाने वाले विकल्प। रिक्त हो सकता है. |

### यह सभी देखें

* class [PrintOptions](../../../aspose.note.saving/printoptions/)
* class [Document](../)
* नाम स्थान [Aspose.Note](../../document/)
* सभा [Aspose.Note](../../../)


