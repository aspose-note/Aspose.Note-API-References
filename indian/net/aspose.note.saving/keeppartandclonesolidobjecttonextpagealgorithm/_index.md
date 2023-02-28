---
title: Class KeepPartAndCloneSolidObjectToNextPageAlgorithm
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.Saving.KeepPartAndCloneSolidObjectToNextPageAlgorithm कक्ष. ऑब्जेक्ट के शर्ष भग क पृष्ठ के नचले भग में जड़त है और पूर्ण ऑब्जेक्ट क अगले पृष्ठ पर क्लन करत है यद यह मूल पृष्ठ में फट नहं हत है
type: docs
weight: 730
url: /hi/net/aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/
---
## KeepPartAndCloneSolidObjectToNextPageAlgorithm class

ऑब्जेक्ट के शीर्ष भाग को पृष्ठ के निचले भाग में जोड़ता है और पूर्ण ऑब्जेक्ट को अगले पृष्ठ पर क्लोन करता है यदि यह मूल पृष्ठ में फिट नहीं होता है।

```csharp
public class KeepPartAndCloneSolidObjectToNextPageAlgorithm : PageSplittingAlgorithm
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm](keeppartandclonesolidobjecttonextpagealgorithm/#constructor)() | का एक नया उदाहरण प्रारंभ करता है`KeepPartAndCloneSolidObjectToNextPageAlgorithm` वर्ग, क्लोन किए गए भाग की डिफ़ॉल्ट ऊंचाई सीमा का उपयोग करते हुए। |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm](keeppartandclonesolidobjecttonextpagealgorithm/#constructor_1)(float) | का एक नया उदाहरण प्रारंभ करता है`KeepPartAndCloneSolidObjectToNextPageAlgorithm` वर्ग, क्लोन किए गए भाग की विशिष्ट ऊंचाई सीमा का उपयोग करते हुए। |

## गुण

| नाम | विवरण |
| --- | --- |
| [HeightLimitOfClonedPart](../../aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/heightlimitofclonedpart/) { get; } | क्लोन किए गए भाग की ऊंचाई सीमा प्राप्त करता है। |

## खेत

| नाम | विवरण |
| --- | --- |
| const [DefaultHeightLimitOfClonedPart](../../aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/defaultheightlimitofclonedpart/) | क्लोन किए गए भाग का डिफ़ॉल्ट अधिकतम आकार। |

### उदाहरण

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

* class [PageSplittingAlgorithm](../pagesplittingalgorithm/)
* नाम स्थान [Aspose.Note.Saving](../../aspose.note.saving/)
* सभा [Aspose.Note](../../)


