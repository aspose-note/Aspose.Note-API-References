---
title: Page.IsConflictPage
second_title: Aspose.Note per .NET API Reference
description: Page proprietà. Ottiene o imposta un valore che indica se questa pagina è una pagina in conflitto.
type: docs
weight: 50
url: /it/net/aspose.note/page/isconflictpage/
---
## Page.IsConflictPage property

Ottiene o imposta un valore che indica se questa pagina è una pagina in conflitto.

```csharp
public bool IsConflictPage { get; set; }
```

### Osservazioni

La pagina in conflitto si verifica quando due utenti tentano di aggiornare lo stesso contenuto. In questo caso le modifiche del primo utente vengono scritte come al solito. Ma le modifiche di un altro utente non possono essere unite. Quindi viene creata solo una copia della pagina e contrassegnato come conflitto.

In questa versione i conflitti vengono risolti a favore delle modifiche del primo utente. Quindi, se il documento ha pagine in conflitto, verranno mostrate nella cronologia ma verranno saltate al salvataggio. È possibile reimpostare questo flag per salvare queste pagine nella storia come al solito.

Un esempio dettagliato della pagina di manipolazione per conflitto è disponibile nella documentazione online.

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

* class [Page](../)
* spazio dei nomi [Aspose.Note](../../page/)
* assemblea [Aspose.Note](../../../)


