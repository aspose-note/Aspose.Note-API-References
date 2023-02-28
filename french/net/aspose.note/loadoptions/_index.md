---
title: Class LoadOptions
second_title: Référence de l'API Aspose.Note pour .NET
description: Aspose.Note.LoadOptions classe. Options utilisées pour charger un document.
type: docs
weight: 320
url: /fr/net/aspose.note/loadoptions/
---
## LoadOptions class

Options utilisées pour charger un document.

```csharp
public class LoadOptions
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [LoadOptions](loadoptions/)() | Default_Constructor |

## Propriétés

| Nom | La description |
| --- | --- |
| [DocumentPassword](../../aspose.note/loadoptions/documentpassword/) { get; set; } | Obtient ou définit un mot de passe pour le contenu du document chiffré. La valeur est ignorée si le document n'est pas protégé par un mot de passe. |
| [LoadHistory](../../aspose.note/loadoptions/loadhistory/) { get; set; } | Obtient ou définit une valeur indiquant si un chargeur de document doit ignorer l'historique. Utilisez cette option pour réduire l'utilisation de la mémoire et du processeur. La valeur par défaut est`vrai` . |

### Exemples

Montre comment un document chiffré.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

Montre comment créer un bloc-notes chiffré.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

Montre comment obtenir l'historique de la page.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Pages();

// Charger le document OneNote
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Récupère la première page
Page firstPage = document.FirstChild;
foreach (Page pageRevision in document.GetPageHistory(firstPage))
{
    /*Use pageRevision like a regular page.*/
    Console.WriteLine("LastModifiedTime: {0}", pageRevision.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", pageRevision.CreationTime);
    Console.WriteLine("Title: {0}", pageRevision.Title);
    Console.WriteLine("Level: {0}", pageRevision.Level);
    Console.WriteLine("Author: {0}", pageRevision.Author);
    Console.WriteLine();
}
```

### Voir également

* espace de noms [Aspose.Note](../../aspose.note/)
* Assemblée [Aspose.Note](../../)


