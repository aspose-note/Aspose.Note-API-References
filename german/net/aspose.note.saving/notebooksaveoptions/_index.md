---
title: Class NotebookSaveOptions
second_title: Aspose.Note für .NET-API-Referenz
description: Aspose.Note.Saving.NotebookSaveOptions klas. Eine abstrakte Basisklasse die Optionen zum Speichern von Notizbüchern für ein bestimmtes Format darstellt.
type: docs
weight: 790
url: /de/net/aspose.note.saving/notebooksaveoptions/
---
## NotebookSaveOptions class

Eine abstrakte Basisklasse, die Optionen zum Speichern von Notizbüchern für ein bestimmtes Format darstellt.

```csharp
public abstract class NotebookSaveOptions
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob untergeordnete Dokumente explizit gespeichert werden sollen. |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob die Hierarchie der untergeordneten Notizbücher abgeflacht gespeichert wird. |
| abstract [SaveFormat](../../aspose.note.saving/notebooksaveoptions/saveformat/) { get; } | Ruft das Format ab, in dem das Notizbuch gespeichert ist. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| abstract [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions/getdocumentsaveoptions/)() | Ruft die Speicheroptionen für alle untergeordneten Dokumente des Notizbuchs ab. |

### Beispiele

Zeigt, wie ein reduziertes Notizbuch im PDF-Format gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Ein OneNote-Notizbuch laden
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Speichern Sie das Notizbuch
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

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

Zeigt, wie ein reduziertes Notizbuch als Bild gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Ein OneNote-Notizbuch laden
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Speichern Sie das Notizbuch
notebook.Save(dataDir, notebookSaveOptions);
```

### Siehe auch

* namensraum [Aspose.Note.Saving](../../aspose.note.saving/)
* Montage [Aspose.Note](../../)


