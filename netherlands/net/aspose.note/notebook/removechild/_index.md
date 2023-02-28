---
title: Notebook.RemoveChild
second_title: Aspose.Note voor .NET API-referentie
description: Notebook methode. Verwijdert het onderliggende knooppunt.
type: docs
weight: 140
url: /nl/net/aspose.note/notebook/removechild/
---
## Notebook.RemoveChild method

Verwijdert het onderliggende knooppunt.

```csharp
public INotebookChildNode RemoveChild(INotebookChildNode oldChild)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| oldChild | INotebookChildNode | Het knooppunt dat moet worden verwijderd. |

### Winstwaarde

Het verwijderde knooppunt.

### Voorbeelden

Laat zien hoe u toegang krijgt tot alle secties vanuit een notitieblok.

```csharp
string inputFile = "notebook.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

Notebook rootNotebook = new Notebook(dataDir + inputFile);

IList<Document> allDocuments = rootNotebook.GetChildNodes<Document>();
foreach (Document document in allDocuments) 
{
    Console.WriteLine(document.DisplayName);
}
```

Laat zien hoe u een sectie uit een notitieblok verwijdert.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Laad een OneNote-notitieblok
var notebook = new Notebook(dataDir + "test.onetoc2");

// Blader door de onderliggende knooppunten om het gewenste onderliggende item te zoeken
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // Verwijder het onderliggende item uit het notitieblok
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// Sla het notitieblok op
notebook.Save(dataDir);
```

Laat zien hoe u een notitieblok opslaat.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_NoteBook();

var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = false });

notebook.Save(dataDir + "notebook_out.onetoc2", new NotebookOneSaveOptions() { DeferredSaving = true});

if (notebook.Any())
{
    var childDocument0 = notebook[0] as Document;

    childDocument0.Save(dataDir + "Not Locked_out.one");

    var childDocument1 = notebook[1] as Document;

    childDocument1.Save(dataDir + "Locked Pass1_out.one", new OneSaveOptions() { DocumentPassword = "pass" });

    var childDocument2 = notebook[2] as Document;

    childDocument2.Save(dataDir + "Locked Pass2_out.one", new OneSaveOptions() { DocumentPassword = "pass2" });
}
```

### Zie ook

* interface [INotebookChildNode](../../inotebookchildnode/)
* class [Notebook](../)
* naamruimte [Aspose.Note](../../notebook/)
* montage [Aspose.Note](../../../)


