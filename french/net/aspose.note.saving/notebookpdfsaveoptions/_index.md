---
title: Class NotebookPdfSaveOptions
second_title: Référence de l'API Aspose.Note pour .NET
description: Aspose.Note.Saving.NotebookPdfSaveOptions classe. Permet de spécifier des options supplémentaires lors du rendu des pages du blocnotes au format PDF.
type: docs
weight: 780
url: /fr/net/aspose.note.saving/notebookpdfsaveoptions/
---
## NotebookPdfSaveOptions class

Permet de spécifier des options supplémentaires lors du rendu des pages du bloc-notes au format PDF.

```csharp
public class NotebookPdfSaveOptions : NotebookSaveOptions<PdfSaveOptions>
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [NotebookPdfSaveOptions](notebookpdfsaveoptions/)() | Default_Constructor |

## Propriétés

| Nom | La description |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | Obtient ou définit une valeur indiquant si les documents enfants doivent être enregistrés explicitement. |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } |  |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | Obtient ou définit une valeur indiquant si la hiérarchie des enfants du bloc-notes est enregistrée à plat. |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } |  |

## Méthodes

| Nom | La description |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() |  |

### Exemples

Montre comment enregistrer un bloc-notes au format pdf avec les options spécifiées.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Charger un bloc-notes OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookPdfSaveOptions();

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Enregistrer le bloc-notes
notebook.Save(dataDir, notebookSaveOptions);
```

### Voir également

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../notebooksaveoptions-1/)
* class [PdfSaveOptions](../pdfsaveoptions/)
* espace de noms [Aspose.Note.Saving](../../aspose.note.saving/)
* Assemblée [Aspose.Note](../../)


