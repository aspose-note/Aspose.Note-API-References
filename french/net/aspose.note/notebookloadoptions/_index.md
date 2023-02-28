---
title: Class NotebookLoadOptions
second_title: Référence de l'API Aspose.Note pour .NET
description: Aspose.Note.NotebookLoadOptions classe. Options utilisées pour charger un blocnotes.
type: docs
weight: 420
url: /fr/net/aspose.note/notebookloadoptions/
---
## NotebookLoadOptions class

Options utilisées pour charger un bloc-notes.

```csharp
public class NotebookLoadOptions
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [NotebookLoadOptions](notebookloadoptions/)() | Default_Constructor |

## Propriétés

| Nom | La description |
| --- | --- |
| [DeferredLoading](../../aspose.note/notebookloadoptions/deferredloading/) { get; set; } | Obtient ou définit une valeur indiquant si les documents enfants doivent être chargés explicitement ultérieurement. |
| [InstantLoading](../../aspose.note/notebookloadoptions/instantloading/) { get; set; } | Obtient ou définit une valeur indiquant si les documents enfants doivent être chargés pendant le chargement du document parent. |

### Exemples

Montre comment créer un bloc-notes chiffré.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

### Voir également

* espace de noms [Aspose.Note](../../aspose.note/)
* Assemblée [Aspose.Note](../../)


