---
title: Class LoadOptions
second_title: Aspose.Note för .NET API-referens
description: Aspose.Note.LoadOptions klass. Alternativ som används för att ladda ett dokument.
type: docs
weight: 320
url: /sv/net/aspose.note/loadoptions/
---
## LoadOptions class

Alternativ som används för att ladda ett dokument.

```csharp
public class LoadOptions
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [LoadOptions](loadoptions/)() | Default_Constructor |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [DocumentPassword](../../aspose.note/loadoptions/documentpassword/) { get; set; } | Hämtar eller ställer in ett lösenord för det krypterade dokumentinnehållet. Värdet ignoreras om dokumentet inte är lösenordsskyddat. |
| [LoadHistory](../../aspose.note/loadoptions/loadhistory/) { get; set; } | Hämtar eller ställer in ett värde som anger om en dokumentladdare ska ignorera historiken. Använd det här alternativet för att minska minne och CPU-användning. Standardvärdet är`Sann` . |

### Exempel

Visar hur man gör ett krypterat dokument.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

Visar hur man använder en krypterad anteckningsbok.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

Visar hur man hämtar sidans historik.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Pages();

// Ladda OneNote-dokument
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Få första sidan
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

### Se även

* namnutrymme [Aspose.Note](../../aspose.note/)
* hopsättning [Aspose.Note](../../)


