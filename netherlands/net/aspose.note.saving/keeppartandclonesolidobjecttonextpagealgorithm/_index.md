---
title: Class KeepPartAndCloneSolidObjectToNextPageAlgorithm
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.Saving.KeepPartAndCloneSolidObjectToNextPageAlgorithm klas. Voegt het bovenste deel van het object toe aan de onderkant van de pagina en kloont het volledige object naar de volgende pagina voor het geval het niet op de originele pagina past.
type: docs
weight: 730
url: /nl/net/aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/
---
## KeepPartAndCloneSolidObjectToNextPageAlgorithm class

Voegt het bovenste deel van het object toe aan de onderkant van de pagina en kloont het volledige object naar de volgende pagina voor het geval het niet op de originele pagina past.

```csharp
public class KeepPartAndCloneSolidObjectToNextPageAlgorithm : PageSplittingAlgorithm
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm](keeppartandclonesolidobjecttonextpagealgorithm/#constructor)() | Initialiseert een nieuw exemplaar van het`KeepPartAndCloneSolidObjectToNextPageAlgorithm` klasse, met standaard hoogtelimiet van gekloond onderdeel. |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm](keeppartandclonesolidobjecttonextpagealgorithm/#constructor_1)(float) | Initialiseert een nieuw exemplaar van het`KeepPartAndCloneSolidObjectToNextPageAlgorithm` klasse, met behulp van een specifieke hoogtelimiet van gekloond onderdeel. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [HeightLimitOfClonedPart](../../aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/heightlimitofclonedpart/) { get; } | Haalt de hoogtelimiet van gekloond onderdeel op. |

## Velden

| Naam | Beschrijving |
| --- | --- |
| const [DefaultHeightLimitOfClonedPart](../../aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/defaultheightlimitofclonedpart/) | De standaard maximale grootte van gekloond onderdeel. |

### Voorbeelden

Wanneer lange OneNote-pagina's in pdf-indeling worden opgeslagen, worden ze over pagina's verdeeld. Het voorbeeld laat zien hoe u de splitsingslogica configureert van objecten die zich op pagina-einden bevinden.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// of
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

Wanneer lange OneNote-pagina's in pdf-indeling worden opgeslagen, worden ze over pagina's verdeeld. Het voorbeeld laat zien hoe u de splitsingslogica configureert van objecten die zich op pagina-einden bevinden.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// Of
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// Of
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// Of
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// Of
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

### Zie ook

* class [PageSplittingAlgorithm](../pagesplittingalgorithm/)
* naamruimte [Aspose.Note.Saving](../../aspose.note.saving/)
* montage [Aspose.Note](../../)


