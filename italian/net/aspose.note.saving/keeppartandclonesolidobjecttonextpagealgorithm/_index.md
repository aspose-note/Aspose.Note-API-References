---
title: Class KeepPartAndCloneSolidObjectToNextPageAlgorithm
second_title: Aspose.Note per .NET API Reference
description: Aspose.Note.Saving.KeepPartAndCloneSolidObjectToNextPageAlgorithm classe. Aggiunge la parte superiore delloggetto alla parte inferiore della pagina e clona lintero oggetto nella pagina successiva nel caso in cui non si adatti alla pagina originale.
type: docs
weight: 730
url: /it/net/aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/
---
## KeepPartAndCloneSolidObjectToNextPageAlgorithm class

Aggiunge la parte superiore dell'oggetto alla parte inferiore della pagina e clona l'intero oggetto nella pagina successiva nel caso in cui non si adatti alla pagina originale.

```csharp
public class KeepPartAndCloneSolidObjectToNextPageAlgorithm : PageSplittingAlgorithm
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm](keeppartandclonesolidobjecttonextpagealgorithm/#constructor)() | Inizializza una nuova istanza di`KeepPartAndCloneSolidObjectToNextPageAlgorithm` classe, utilizzando il limite di altezza predefinito della parte clonata. |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm](keeppartandclonesolidobjecttonextpagealgorithm/#constructor_1)(float) | Inizializza una nuova istanza di`KeepPartAndCloneSolidObjectToNextPageAlgorithm` classe, utilizzando il limite di altezza specifico della parte clonata. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [HeightLimitOfClonedPart](../../aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/heightlimitofclonedpart/) { get; } | Ottiene il limite di altezza della parte clonata. |

## Campi

| Nome | Descrizione |
| --- | --- |
| const [DefaultHeightLimitOfClonedPart](../../aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/defaultheightlimitofclonedpart/) | La dimensione massima predefinita della parte clonata. |

### Esempi

Quando le pagine lunghe di OneNote vengono salvate in formato pdf, vengono suddivise tra le pagine. L'esempio mostra come configurare la logica di suddivisione degli oggetti posizionati sulle interruzioni di pagina.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// O
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

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


