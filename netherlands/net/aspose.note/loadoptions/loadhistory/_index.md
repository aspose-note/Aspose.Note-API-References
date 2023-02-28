---
title: LoadOptions.LoadHistory
second_title: Aspose.Note voor .NET API-referentie
description: LoadOptions eigendom. Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of een documentlader de geschiedenis moet negeren. Gebruik deze optie om geheugen en CPUgebruik te verminderen. Standaardwaarde isWAAR .
type: docs
weight: 30
url: /nl/net/aspose.note/loadoptions/loadhistory/
---
## LoadOptions.LoadHistory property

Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of een documentlader de geschiedenis moet negeren. Gebruik deze optie om geheugen- en CPU-gebruik te verminderen. Standaardwaarde is`WAAR` .

```csharp
public bool LoadHistory { get; set; }
```

### Voorbeelden

Laat zien hoe u de geschiedenis van de pagina kunt ophalen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Pages();

// Laad OneNote-document
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Haal de eerste pagina op
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

### Zie ook

* class [LoadOptions](../)
* naamruimte [Aspose.Note](../../loadoptions/)
* montage [Aspose.Note](../../../)


