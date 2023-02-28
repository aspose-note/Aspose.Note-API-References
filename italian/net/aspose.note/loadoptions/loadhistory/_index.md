---
title: LoadOptions.LoadHistory
second_title: Aspose.Note per .NET API Reference
description: LoadOptions proprietà. Ottiene o imposta un valore che indica se un caricatore di documenti deve ignorare la cronologia. Utilizzare questa opzione per ridurre lutilizzo della memoria e della CPU. Il valore predefinito èVERO .
type: docs
weight: 30
url: /it/net/aspose.note/loadoptions/loadhistory/
---
## LoadOptions.LoadHistory property

Ottiene o imposta un valore che indica se un caricatore di documenti deve ignorare la cronologia. Utilizzare questa opzione per ridurre l'utilizzo della memoria e della CPU. Il valore predefinito è`VERO` .

```csharp
public bool LoadHistory { get; set; }
```

### Esempi

Mostra come ottenere la cronologia della pagina.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Pages();

// Carica il documento OneNote
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Ottieni la prima pagina
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

### Guarda anche

* class [LoadOptions](../)
* spazio dei nomi [Aspose.Note](../../loadoptions/)
* assemblea [Aspose.Note](../../../)


