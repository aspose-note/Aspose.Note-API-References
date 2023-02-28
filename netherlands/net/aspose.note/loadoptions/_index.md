---
title: Class LoadOptions
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.LoadOptions klas. Opties gebruikt om een document te laden.
type: docs
weight: 320
url: /nl/net/aspose.note/loadoptions/
---
## LoadOptions class

Opties gebruikt om een document te laden.

```csharp
public class LoadOptions
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [LoadOptions](loadoptions/)() | De standaard constructeur. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [DocumentPassword](../../aspose.note/loadoptions/documentpassword/) { get; set; } | Haalt of stelt een wachtwoord in voor de versleutelde documentinhoud. Waarde wordt genegeerd als het document niet met een wachtwoord is beveiligd. |
| [LoadHistory](../../aspose.note/loadoptions/loadhistory/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of een documentlader de geschiedenis moet negeren. Gebruik deze optie om geheugen- en CPU-gebruik te verminderen. Standaardwaarde is`WAAR` . |

### Voorbeelden

Laat zien hoe u een gecodeerd document maakt.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

Laat zien hoe je een versleuteld notitieboekje gebruikt.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
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

* naamruimte [Aspose.Note](../../aspose.note/)
* montage [Aspose.Note](../../)


