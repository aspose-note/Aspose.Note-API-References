---
title: Class RevisionSummary
second_title: Aspose.Note per .NET API Reference
description: Aspose.Note.RevisionSummary classe. Rappresenta un riepilogo per la revisione del nodo.
type: docs
weight: 520
url: /it/net/aspose.note/revisionsummary/
---
## RevisionSummary class

Rappresenta un riepilogo per la revisione del nodo.

```csharp
public class RevisionSummary
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [RevisionSummary](revisionsummary/)() | Default_Costruttore |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AuthorMostRecent](../../aspose.note/revisionsummary/authormostrecent/) { get; set; } | Ottiene o imposta l'autore più recente. |
| [LastModifiedTime](../../aspose.note/revisionsummary/lastmodifiedtime/) { get; set; } | Ottiene o imposta l'ora dell'ultima modifica. |

### Esempi

Mostra come modificare le meta informazioni della pagina.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Pages();

// Carica il documento OneNote e ottieni il primo figlio           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

// Lettura del riepilogo della revisione del contenuto per questa pagina
var pageRevisionInfo = page.PageContentRevisionSummary;

Console.WriteLine(string.Format(
    "Author:\t{0}\nModified:\t{1}",
    pageRevisionInfo.AuthorMostRecent,
    pageRevisionInfo.LastModifiedTime.ToString("dd.MM.yyyy HH:mm:ss")));

// Aggiorna il riepilogo delle revisioni della pagina per questa pagina
pageRevisionInfo.AuthorMostRecent = "New Author";
pageRevisionInfo.LastModifiedTime = DateTime.Now;

document.Save(dataDir + "WorkingWithPageRevisions_out.one");
```

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

* spazio dei nomi [Aspose.Note](../../aspose.note/)
* assemblea [Aspose.Note](../../)


