---
title: PdfSaveOptions
second_title: Aspose.Note für .NET-API-Referenz
description: Ermöglicht das Festlegen zusätzlicher Optionen beim Rendern von Dokumentseiten in PDF.
type: docs
weight: 820
url: /de/net/aspose.note.saving/pdfsaveoptions/
---
## PdfSaveOptions class

Ermöglicht das Festlegen zusätzlicher Optionen beim Rendern von Dokumentseiten in PDF.

```csharp
public sealed class PdfSaveOptions : SaveOptions
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions)() | Default_Constructor |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem) { get; set; } | Ruft die beim Speichern zu verwendenden Schrifteinstellungen ab oder legt sie fest |
| [ImageCompression](../../aspose.note.saving/pdfsaveoptions/imagecompression) { get; set; } | Ruft den auf Bilder in der PDF-Datei angewendeten Komprimierungstyp ab oder legt ihn fest. |
| [JpegQuality](../../aspose.note.saving/pdfsaveoptions/jpegquality) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der die Qualität der JPEG-Bilder im PDF-Dokument bestimmt. Der Wert kann zwischen 0 und 100 liegen, wobei 0 die schlechteste Qualität, aber maximale Komprimierung und 100 die beste Qualität, aber minimale Komprimierung bedeutet. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount) { get; set; } | Ruft die Anzahl der zu speichernden Seiten ab oder legt sie fest. Standardmäßig istMaxValue , was bedeutet, dass alle Seiten des Dokuments gerendert werden. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex) { get; set; } | Ruft den Index der ersten zu speichernden Seite ab oder legt ihn fest. Standardmäßig ist 0. |
| [PageSplittingAlgorithm](../../aspose.note.saving/pdfsaveoptions/pagesplittingalgorithm) { get; set; } | Ruft den für die Seitenaufteilung verwendeten Algorithmus ab oder legt ihn fest. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat) { get; } | Ruft das Format ab, in dem das Dokument gespeichert ist. |

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

Zeigt, wie ein Dokument im PDF-Format gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// PdfSaveOptions-Objekt initialisieren
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Seitenindex der ersten zu speichernden Seite setzen
                              PageIndex = 0,

                              // Seitenanzahl festlegen
                              PageCount = 1,
                          };

// Dokument als PDF speichern
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Zeigt, wie Sie ein Dokument im PDF-Format mit bestimmten Einstellungen speichern.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// PdfSaveOptions-Objekt initialisieren
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // JPEG-Komprimierung verwenden
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Qualität für JPEG-Komprimierung
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
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

* class [SaveOptions](../saveoptions)
* namensraum [Aspose.Note.Saving](../../aspose.note.saving)
* Montage [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
