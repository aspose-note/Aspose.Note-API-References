---
title: CompositeNode1.FirstChild
second_title: Référence de l'API Aspose.Note pour .NET
description: CompositeNode propriété. Obtient le premier nœud enfant de ce nœud.
type: docs
weight: 10
url: /fr/net/aspose.note/compositenode-1/firstchild/
---
## CompositeNode&lt;T&gt;.FirstChild property

Obtient le premier nœud enfant de ce nœud.

```csharp
public T FirstChild { get; }
```

### Exemples

Montre comment vérifier si une page est une page en conflit (c'est-à-dire qu'elle contient des modifications que OneNote n'a pas pu fusionner automatiquement).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// Charger le document OneNote
Document doc = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

var history = doc.GetPageHistory(doc.FirstChild);
for (int i = 0; i < history.Count; i++)
{
    var historyPage = history[i];
    Console.Write("    {0}. Author: {1}, {2:dd.MM.yyyy hh.mm.ss}",
                    i,
                    historyPage.PageContentRevisionSummary.AuthorMostRecent,
                    historyPage.PageContentRevisionSummary.LastModifiedTime);
    Console.WriteLine(historyPage.IsConflictPage ? ", IsConflict: true" : string.Empty);

    // Par défaut, les pages en conflit sont simplement ignorées lors de l'enregistrement.
    // Si vous le marquez comme non conflictuel, il sera enregistré comme d'habitude dans l'historique.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

### Voir également

* class [CompositeNode&lt;T&gt;](../)
* espace de noms [Aspose.Note](../../compositenode-1/)
* Assemblée [Aspose.Note](../../../)


