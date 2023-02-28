---
title: LoadOptions.LoadHistory
second_title: Aspose.Note für .NET-API-Referenz
description: LoadOptions eigendom. Ruft einen Wert ab oder legt einen Wert fest der angibt ob ein Dokumentladeprogramm den Verlauf ignorieren soll. Verwenden Sie diese Option um die Speicher und CPUAuslastung zu verringern. Der Standardwert istWAHR .
type: docs
weight: 30
url: /de/net/aspose.note/loadoptions/loadhistory/
---
## LoadOptions.LoadHistory property

Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob ein Dokumentladeprogramm den Verlauf ignorieren soll. Verwenden Sie diese Option, um die Speicher- und CPU-Auslastung zu verringern. Der Standardwert ist`WAHR` .

```csharp
public bool LoadHistory { get; set; }
```

### Beispiele

Zeigt, wie man den Seitenverlauf erhält.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote-Dokument laden
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Erste Seite abrufen
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

### Siehe auch

* class [LoadOptions](../)
* namensraum [Aspose.Note](../../loadoptions/)
* Montage [Aspose.Note](../../../)


