---
title: Class KeepPartAndCloneSolidObjectToNextPageAlgorithm
second_title: Aspose.Note för .NET API-referens
description: Aspose.Note.Saving.KeepPartAndCloneSolidObjectToNextPageAlgorithm klass. Lägger till objektets övre del längst ner på sidan och klonar hela objektet till nästa sida om det inte får plats på originalsidan.
type: docs
weight: 730
url: /sv/net/aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/
---
## KeepPartAndCloneSolidObjectToNextPageAlgorithm class

Lägger till objektets övre del längst ner på sidan och klonar hela objektet till nästa sida om det inte får plats på originalsidan.

```csharp
public class KeepPartAndCloneSolidObjectToNextPageAlgorithm : PageSplittingAlgorithm
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm](keeppartandclonesolidobjecttonextpagealgorithm/#constructor)() | Initierar en ny instans av`KeepPartAndCloneSolidObjectToNextPageAlgorithm` klass, med standardhöjdgräns för klonad del. |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm](keeppartandclonesolidobjecttonextpagealgorithm/#constructor_1)(float) | Initierar en ny instans av`KeepPartAndCloneSolidObjectToNextPageAlgorithm` klass, med specifik höjdgräns för den klonade delen. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [HeightLimitOfClonedPart](../../aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/heightlimitofclonedpart/) { get; } | Hämtar höjdgränsen för den klonade delen. |

## Fält

| namn | Beskrivning |
| --- | --- |
| const [DefaultHeightLimitOfClonedPart](../../aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/defaultheightlimitofclonedpart/) | Standardmaxstorleken för den klonade delen. |

### Exempel

När långa OneNote-sidor sparas i pdf-format delas de upp på sidor. Exemplet visar hur man konfigurerar uppdelningslogiken för objekt som finns på sidavbrott.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// eller
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

När långa OneNote-sidor sparas i pdf-format delas de upp på sidor. Exemplet visar hur man konfigurerar uppdelningslogiken för objekt som finns på sidavbrott.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// Eller
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// Eller
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// Eller
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// Eller
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

### Se även

* class [PageSplittingAlgorithm](../pagesplittingalgorithm/)
* namnutrymme [Aspose.Note.Saving](../../aspose.note.saving/)
* hopsättning [Aspose.Note](../../)


