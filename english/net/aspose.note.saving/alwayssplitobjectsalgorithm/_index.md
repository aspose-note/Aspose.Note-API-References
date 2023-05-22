---
title: Class AlwaysSplitObjectsAlgorithm
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Saving.AlwaysSplitObjectsAlgorithm class. Splits an object into several parts in case it doesnt fit in original page
type: docs
weight: 600
url: /net/aspose.note.saving/alwayssplitobjectsalgorithm/
---
## AlwaysSplitObjectsAlgorithm class

Splits an object into several parts in case it doesn't fit in original page.

```csharp
public class AlwaysSplitObjectsAlgorithm : PageSplittingAlgorithm
```

## Constructors

| Name | Description |
| --- | --- |
| [AlwaysSplitObjectsAlgorithm](alwayssplitobjectsalgorithm/)() | The default constructor. |

## Examples

When long OneNote pages are saved in pdf format they are split across pages. The example shows how to configure the splitting logic of objects located on page's breaks.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// Or
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// Or
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// Or
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// Or
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

### See Also

* class [PageSplittingAlgorithm](../pagesplittingalgorithm/)
* namespace [Aspose.Note.Saving](../../aspose.note.saving/)
* assembly [Aspose.Note](../../)


