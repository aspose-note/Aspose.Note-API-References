---
title: Class AlwaysSplitObjectsAlgorithm
second_title: Aspose.Note per .NET API Reference
description: Aspose.Note.Saving.AlwaysSplitObjectsAlgorithm classe. Divide un oggetto in più parti nel caso in cui non si adatta alla pagina originale.
type: docs
weight: 550
url: /it/net/aspose.note.saving/alwayssplitobjectsalgorithm/
---
## AlwaysSplitObjectsAlgorithm class

Divide un oggetto in più parti nel caso in cui non si adatta alla pagina originale.

```csharp
public class AlwaysSplitObjectsAlgorithm : PageSplittingAlgorithm
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [AlwaysSplitObjectsAlgorithm](alwayssplitobjectsalgorithm/)() | Default_Costruttore |

### Esempi

Quando le pagine lunghe di OneNote vengono salvate in formato pdf, vengono suddivise tra le pagine. L'esempio mostra come configurare la logica di suddivisione degli oggetti posti sulle interruzioni di pagina.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// O
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// O
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// O
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// O
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

### Guarda anche

* class [PageSplittingAlgorithm](../pagesplittingalgorithm/)
* spazio dei nomi [Aspose.Note.Saving](../../aspose.note.saving/)
* assemblea [Aspose.Note](../../)


