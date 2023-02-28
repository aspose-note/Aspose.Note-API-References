---
title: CompositeNode1.FirstChild
second_title: Aspose.Note per .NET API Reference
description: CompositeNode proprietà. Ottiene il primo nodo figlio di questo nodo.
type: docs
weight: 10
url: /it/net/aspose.note/compositenode-1/firstchild/
---
## CompositeNode&lt;T&gt;.FirstChild property

Ottiene il primo nodo figlio di questo nodo.

```csharp
public T FirstChild { get; }
```

### Esempi

Mostra come verificare se una pagina è una pagina in conflitto (ovvero presenta modifiche che OneNote non è in grado di unire automaticamente).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// Carica il documento OneNote
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

    // Per impostazione predefinita, le pagine in conflitto vengono semplicemente saltate al salvataggio.
    // Se contrassegnalo come non in conflitto, verrà salvato come al solito nella cronologia.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

### Guarda anche

* class [CompositeNode&lt;T&gt;](../)
* spazio dei nomi [Aspose.Note](../../compositenode-1/)
* assemblea [Aspose.Note](../../../)


