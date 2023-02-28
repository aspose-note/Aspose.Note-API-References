---
title: Notebook.DisplayName
second_title: Aspose.Note voor .NET API-referentie
description: Notebook eigendom. Haalt de weergavenaam op of stelt deze in.
type: docs
weight: 40
url: /nl/net/aspose.note/notebook/displayname/
---
## Notebook.DisplayName property

Haalt de weergavenaam op of stelt deze in.

```csharp
public string DisplayName { get; set; }
```

### Voorbeelden

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

### Zie ook

* class [Notebook](../)
* naamruimte [Aspose.Note](../../notebook/)
* montage [Aspose.Note](../../../)


