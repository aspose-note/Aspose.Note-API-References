---
title: Class NotebookImageSaveOptions
second_title: Aspose.Note für .NET-API-Referenz
description: Aspose.Note.Saving.NotebookImageSaveOptions klas. Ermöglicht das Festlegen zusätzlicher Optionen beim Rendern von Notizbuchseiten in Bilder.
type: docs
weight: 760
url: /de/net/aspose.note.saving/notebookimagesaveoptions/
---
## NotebookImageSaveOptions class

Ermöglicht das Festlegen zusätzlicher Optionen beim Rendern von Notizbuchseiten in Bilder.

```csharp
public class NotebookImageSaveOptions : NotebookSaveOptions<ImageSaveOptions>
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [NotebookImageSaveOptions](notebookimagesaveoptions/)(SaveFormat) | Initialisiert eine neue Instanz von`NotebookImageSaveOptions` Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob untergeordnete Dokumente explizit gespeichert werden sollen. |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } |  |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob die Hierarchie der untergeordneten Notizbücher abgeflacht gespeichert wird. |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() |  |

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

Zeigt, wie Notizbuch als Bild mit bestimmten Optionen gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Ein OneNote-Notizbuch laden
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

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

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../notebooksaveoptions-1/)
* class [ImageSaveOptions](../imagesaveoptions/)
* namensraum [Aspose.Note.Saving](../../aspose.note.saving/)
* Montage [Aspose.Note](../../)


