---
title: NotebookSaveOptions1.DocumentSaveOptions
second_title: Référence de l'API Aspose.Note pour .NET
description: NotebookSaveOptions propriété. Obtient ou définit les options denregistrement pour tous les documents enfants du blocnotes.
type: docs
weight: 10
url: /fr/net/aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt;.DocumentSaveOptions property

Obtient ou définit les options d'enregistrement pour tous les documents enfants du bloc-notes.

```csharp
public TDocumentSaveOptions DocumentSaveOptions { get; }
```

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

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../)
* espace de noms [Aspose.Note.Saving](../../notebooksaveoptions-1/)
* Assemblée [Aspose.Note](../../../)


