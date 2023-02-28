---
title: Page.LastModifiedTime
second_title: Aspose.Note voor .NET API-referentie
description: Page eigendom. Haalt of stelt de laatst gewijzigde tijd in.
type: docs
weight: 60
url: /nl/net/aspose.note/page/lastmodifiedtime/
---
## Page.LastModifiedTime property

Haalt of stelt de laatst gewijzigde tijd in.

```csharp
public DateTime LastModifiedTime { get; set; }
```

### Voorbeelden

Laat zien hoe u meta-informatie over een pagina kunt krijgen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Pages();

// Laad het document in Aspose.Note.
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

* class [Page](../)
* naamruimte [Aspose.Note](../../page/)
* montage [Aspose.Note](../../../)


