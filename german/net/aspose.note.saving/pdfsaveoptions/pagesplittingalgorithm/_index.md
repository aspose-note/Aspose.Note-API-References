---
title: PdfSaveOptions.PageSplittingAlgorithm
second_title: Aspose.Note für .NET-API-Referenz
description: PdfSaveOptions eigendom. Ruft den für die Seitenaufteilung verwendeten Algorithmus ab oder legt ihn fest.
type: docs
weight: 50
url: /de/net/aspose.note.saving/pdfsaveoptions/pagesplittingalgorithm/
---
## PdfSaveOptions.PageSplittingAlgorithm property

Ruft den für die Seitenaufteilung verwendeten Algorithmus ab oder legt ihn fest.

```csharp
public PageSplittingAlgorithm PageSplittingAlgorithm { get; set; }
```

### Eigentumswert

Die`PageSplittingAlgorithm` .

### Beispiele

Zeigt, wie Notizbücher im PDF-Format mit den angegebenen Optionen gespeichert werden.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Ein OneNote-Notizbuch laden
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookPdfSaveOptions();

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Speichern Sie das Notizbuch
notebook.Save(dataDir, notebookSaveOptions);
```

Wenn lange OneNote-Seiten im PDF-Format gespeichert werden, werden sie auf Seiten aufgeteilt. Das Beispiel zeigt, wie die Aufteilungslogik von Objekten konfiguriert wird, die sich auf Seitenumbrüchen befinden.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// oder
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

Wenn lange OneNote-Seiten im PDF-Format gespeichert werden, werden sie auf Seiten aufgeteilt. Das Beispiel zeigt, wie die Aufteilungslogik von Objekten konfiguriert wird, die sich auf Seitenumbrüchen befinden.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// Oder
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// Oder
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// Oder
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// Oder
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

### Siehe auch

* class [PageSplittingAlgorithm](../../pagesplittingalgorithm/)
* class [PdfSaveOptions](../)
* namensraum [Aspose.Note.Saving](../../pdfsaveoptions/)
* Montage [Aspose.Note](../../../)


