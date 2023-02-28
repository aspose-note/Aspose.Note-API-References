---
title: Class AlwaysSplitObjectsAlgorithm
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.Saving.AlwaysSplitObjectsAlgorithm कक्ष. मूल पृष्ठ में फट नहं हने क स्थत में कस वस्तु क कई भगं में वभजत करत है
type: docs
weight: 550
url: /hi/net/aspose.note.saving/alwayssplitobjectsalgorithm/
---
## AlwaysSplitObjectsAlgorithm class

मूल पृष्ठ में फिट नहीं होने की स्थिति में किसी वस्तु को कई भागों में विभाजित करता है।

```csharp
public class AlwaysSplitObjectsAlgorithm : PageSplittingAlgorithm
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [AlwaysSplitObjectsAlgorithm](alwayssplitobjectsalgorithm/)() | डिफ़ॉल्ट कंस्ट्रक्टर। |

### उदाहरण

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


