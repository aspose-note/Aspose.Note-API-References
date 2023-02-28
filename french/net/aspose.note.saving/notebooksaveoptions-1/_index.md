---
title: Class NotebookSaveOptionsTDocumentSaveOptions
second_title: Référence de l'API Aspose.Note pour .NET
description: Aspose.Note.Saving.NotebookSaveOptions1TDocumentSaveOptions classe. Une classe de base abstraite qui représente les options denregistrement du blocnotes pour un format particulier et fournit des options denregistrement communes pour tous les nœuds enfants du document.
type: docs
weight: 800
url: /fr/net/aspose.note.saving/notebooksaveoptions-1/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt; class

Une classe de base abstraite qui représente les options d'enregistrement du bloc-notes pour un format particulier et fournit des options d'enregistrement communes pour tous les nœuds enfants du document.

```csharp
public abstract class NotebookSaveOptions<TDocumentSaveOptions> : NotebookSaveOptions
    where TDocumentSaveOptions : SaveOptions
```

| Paramètre | La description |
| --- | --- |
| TDocumentSaveOptions | Les options d'enregistrement pour tous les documents enfants du bloc-notes. |

## Propriétés

| Nom | La description |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | Obtient ou définit une valeur indiquant si les documents enfants doivent être enregistrés explicitement. |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } | Obtient ou définit les options d'enregistrement pour tous les documents enfants du bloc-notes. |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | Obtient ou définit une valeur indiquant si la hiérarchie des enfants du bloc-notes est enregistrée à plat. |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } | Obtient le format dans lequel le bloc-notes est enregistré. |

## Méthodes

| Nom | La description |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() | Obtient les options d'enregistrement pour tous les documents enfants du bloc-notes. |

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

* class [NotebookSaveOptions](../notebooksaveoptions/)
* class [SaveOptions](../saveoptions/)
* espace de noms [Aspose.Note.Saving](../../aspose.note.saving/)
* Assemblée [Aspose.Note](../../)


