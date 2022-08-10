---
title: FirstChild
second_title: Aspose.Note per .NET API Reference
description: Ottiene il primo nodo figlio di questo nodo.
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

Mostra come verificare se una pagina è una pagina in conflitto (ad es. contiene modifiche che OneNote non è stato in grado di unire automaticamente).

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

    // Per impostazione predefinita, le pagine di conflitto vengono semplicemente saltate durante il salvataggio.
    // Se contrassegnalo come non in conflitto, verrà salvato come al solito nella cronologia.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

### Guarda anche

* class [CompositeNode&lt;T&gt;](../../compositenode-1)
* spazio dei nomi [Aspose.Note](../../compositenode-1)
* assemblea [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->