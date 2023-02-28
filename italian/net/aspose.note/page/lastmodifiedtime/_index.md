---
title: Page.LastModifiedTime
second_title: Aspose.Note per .NET API Reference
description: Page proprietà. Ottiene o imposta lora dellultima modifica.
type: docs
weight: 60
url: /it/net/aspose.note/page/lastmodifiedtime/
---
## Page.LastModifiedTime property

Ottiene o imposta l'ora dell'ultima modifica.

```csharp
public DateTime LastModifiedTime { get; set; }
```

### Esempi

Mostra come ottenere meta informazioni su una pagina.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Pages();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

foreach (Page page in oneFile)
{
    Console.WriteLine("LastModifiedTime: {0}", page.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", page.CreationTime);
    Console.WriteLine("Title: {0}", page.Title);
    Console.WriteLine("Level: {0}", page.Level);
    Console.WriteLine("Author: {0}", page.Author);
    Console.WriteLine();
}
```

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

* class [Page](../)
* spazio dei nomi [Aspose.Note](../../page/)
* assemblea [Aspose.Note](../../../)


