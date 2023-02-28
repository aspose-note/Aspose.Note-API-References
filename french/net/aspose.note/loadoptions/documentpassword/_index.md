---
title: LoadOptions.DocumentPassword
second_title: Référence de l'API Aspose.Note pour .NET
description: LoadOptions propriété. Obtient ou définit un mot de passe pour le contenu du document chiffré. La valeur est ignorée si le document nest pas protégé par un mot de passe.
type: docs
weight: 20
url: /fr/net/aspose.note/loadoptions/documentpassword/
---
## LoadOptions.DocumentPassword property

Obtient ou définit un mot de passe pour le contenu du document chiffré. La valeur est ignorée si le document n'est pas protégé par un mot de passe.

```csharp
public string DocumentPassword { get; set; }
```

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

### Voir également

* class [LoadOptions](../)
* espace de noms [Aspose.Note](../../loadoptions/)
* Assemblée [Aspose.Note](../../../)


