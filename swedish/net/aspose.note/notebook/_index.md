---
title: Notebook
second_title: Aspose.Note för .NET API-referens
description: Representerar en Aspose.Note-anteckningsbok.
type: docs
weight: 390
url: /sv/net/aspose.note/notebook/
---
## Notebook class

Representerar en Aspose.Note-anteckningsbok.

```csharp
public class Notebook : IEnumerable<INotebookChildNode>, INotebookChildNode
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [Notebook](notebook#constructor)() | Initierar en ny instans av[`Notebook`](../notebook) class. |
| [Notebook](notebook#constructor_1)(Stream) | Initierar en ny instans av[`Notebook`](../notebook) class. Öppnar en befintlig OneNote-anteckningsbok från en ström. |
| [Notebook](notebook#constructor_3)(string) | Initierar en ny instans av[`Notebook`](../notebook) class. Öppnar en befintlig OneNote-anteckningsbok från en fil. |
| [Notebook](notebook#constructor_2)(Stream, NotebookLoadOptions) | Initierar en ny instans av[`Notebook`](../notebook) class. Öppnar en befintlig OneNote-anteckningsbok från en ström. Tillåter att ange ytterligare laddningsalternativ. |
| [Notebook](notebook#constructor_4)(string, NotebookLoadOptions) | Initierar en ny instans av[`Notebook`](../notebook)class. Öppnar en befintlig OneNote-anteckningsbok från en fil. Tillåter att ange ytterligare alternativ såsom en laddningsstrategi för barn ("lata"/instant). |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Color](../../aspose.note/notebook/color) { get; set; } | Hämtar eller ställer in färgen. |
| [Count](../../aspose.note/notebook/count) { get; } | Får antalet element som finns i[`Notebook`](../notebook) . |
| [DisplayName](../../aspose.note/notebook/displayname) { get; set; } | Hämtar eller ställer in visningsnamnet. |
| [FileFormat](../../aspose.note/notebook/fileformat) { get; } | Hämtar filformat (OneNote 2010, OneNote Online). |
| [Guid](../../aspose.note/notebook/guid) { get; } | Får objektets globalt unika id. |
| [IsHistoryEnabled](../../aspose.note/notebook/ishistoryenabled) { get; set; } | Hämtar eller ställer in ett värde som anger om historiken är aktiverad. |
| [Item](../../aspose.note/notebook/item) { get; } | Hämtar anteckningsbokens underordnade nod av det givna indexet. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [AppendChild](../../aspose.note/notebook/appendchild)(INotebookChildNode) | Lägger till noden i slutet av listan. |
| [GetChildNodes&lt;T1&gt;](../../aspose.note/notebook/getchildnodes)() | Hämta alla underordnade noder efter nodtyp. |
| [GetEnumerator](../../aspose.note/notebook/getenumerator)() | Returnerar en enumerator som itererar genom underordnade noder av[`Notebook`](../notebook) . |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument)(Stream) | Lägger till en underordnad dokumentnod. Öppnar ett befintligt OneNote-dokument från en ström. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument_2)(string) | Lägger till en underordnad dokumentnod. Öppnar ett befintligt OneNote-dokument från en fil. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument_1)(Stream, LoadOptions) | Lägger till en underordnad dokumentnod. Öppnar ett befintligt OneNote-dokument från en ström. Tillåter att ange ytterligare laddningsalternativ. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument_3)(string, LoadOptions) | Lägger till en underordnad dokumentnod. Öppnar ett befintligt OneNote-dokument från en fil. Tillåter att ange ytterligare laddningsalternativ. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook)(Stream) | Lägger till en underordnad anteckningsboknod. Öppnar en befintlig OneNote-anteckningsbok från en ström. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook_2)(string) | Lägger till en underordnad anteckningsboknod. Öppnar en befintlig OneNote-anteckningsbok från en fil. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook_1)(Stream, NotebookLoadOptions) | Lägger till en underordnad anteckningsboknod. Öppnar en befintlig OneNote-anteckningsbok från en ström. Tillåter att ange ytterligare laddningsalternativ. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook_3)(string, NotebookLoadOptions) | Lägger till en underordnad anteckningsboknod. Öppnar en befintlig OneNote-anteckningsbok från en fil. Tillåter att ange ytterligare laddningsalternativ. |
| [RemoveChild](../../aspose.note/notebook/removechild)(INotebookChildNode) | Tar bort den underordnade noden. |
| [Save](../../aspose.note/notebook/save#save)(Stream) | Sparar OneNote-dokumentet i en ström. |
| [Save](../../aspose.note/notebook/save#save_3)(string) | Sparar OneNote-dokumentet till en fil. |
| [Save](../../aspose.note/notebook/save#save_2)(Stream, NotebookSaveOptions) | Sparar OneNote-dokumentet i en ström med de angivna sparalternativen. |
| [Save](../../aspose.note/notebook/save#save_1)(Stream, SaveFormat) | Sparar OneNote-dokumentet i en ström i det angivna formatet. |
| [Save](../../aspose.note/notebook/save#save_5)(string, NotebookSaveOptions) | Sparar OneNote-dokumentet till en fil med de angivna sparalternativen. |
| [Save](../../aspose.note/notebook/save#save_4)(string, SaveFormat) | Sparar OneNote-dokumentet till en fil i det angivna formatet. |

### Exempel

Visar hur du sparar anteckningsboken.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_NoteBook();

var notebook = new Notebook();

dataDir = dataDir + "test_out.onetoc2";

// Spara anteckningsboken
notebook.Save(dataDir);
```

Visar hur man sparar anteckningsboken i pdf-format.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Ladda en OneNote-anteckningsbok
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Spara anteckningsboken
notebook.Save(dataDir);
```

Visar hur du sparar anteckningsboken som bild.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Ladda en OneNote-anteckningsbok
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToImage_out.png";

// Spara anteckningsboken
notebook.Save(dataDir);
```

Visar hur man hämtar all text från en anteckningsbok.

```csharp
string inputFile = "notebook.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

Notebook rootNotebook = new Notebook(dataDir + inputFile);

IList<RichText> allRichTextNodes = rootNotebook.GetChildNodes<RichText>();
foreach (RichText richTextNode in allRichTextNodes)
{
    Console.WriteLine(richTextNode.Text);
}
```

Visar hur man sparar tillplattad anteckningsbok i pdf-format.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Ladda en OneNote-anteckningsbok
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Spara anteckningsboken
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

Visar hur man itererar genom dokument från en anteckningsbok som laddar dem lätt.

```csharp
string inputFile = "Notizbuch öffnen.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

// Som standard är barnladdning "lat".
Notebook notebook = new Notebook(dataDir + inputFile);

foreach (var notebookChildNode in notebook.OfType<Document>()) 
{
    // Faktisk laddning av det underordnade dokumentet sker endast här.
    // Gör något med barndokument
}
```

Visar hur man lägger till ett nytt avsnitt i en anteckningsbok.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Ladda en OneNote-anteckningsbok
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Lägg till ett nytt barn till anteckningsboken
notebook.AppendChild(new Document(dataDir + "Neuer Abschnitt 1.one"));

dataDir = dataDir + "AddChildNode_out.onetoc2";

// Spara anteckningsboken
notebook.Save(dataDir);
```

Visar hur man laddar anteckningsboken från en ström.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
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

Visar hur du sparar anteckningsboken som bild med angivna alternativ.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Ladda en OneNote-anteckningsbok
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// Spara anteckningsboken
notebook.Save(dataDir, notebookSaveOptions);
```

Visar hur man sparar tillplattad anteckningsbok som bild.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Ladda en OneNote-anteckningsbok
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Spara anteckningsboken
notebook.Save(dataDir, notebookSaveOptions);
```

Visar hur man tar bort ett avsnitt från en anteckningsbok.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Ladda en OneNote-anteckningsbok
var notebook = new Notebook(dataDir + "test.onetoc2");

// Gå igenom dess underordnade noder för att söka efter önskat underordnat objekt
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // Ta bort det underordnade föremålet från anteckningsboken
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// Spara anteckningsboken
notebook.Save(dataDir);
```

Visar hur man itererar genom förinstallerade dokument i en anteckningsbok.

```csharp
// Som standard är barnladdning "lat".
// Därför har för omedelbar laddning skett,
// det är nödvändigt att ställa in flaggan NotebookLoadOptions.InstantLoading.
NotebookLoadOptions loadOptions = new NotebookLoadOptions { InstantLoading = true };

String inputFile = "Notizbuch öffnen.onetoc2";
String dataDir = RunExamples.GetDataDir_NoteBook();
Notebook notebook = new Notebook(dataDir + inputFile, loadOptions);

// Alla underordnade dokument är redan inlästa.
foreach (INotebookChildNode notebookChildNode in notebook.OfType<Document>()) 
{
   // Gör något med barndokument
}
```

Visar hur man går igenom innehållet i en anteckningsbok.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = "Open Notebook.onetoc2";
try
{
    var notebook = new Notebook(dataDir + fileName);
    foreach (var notebookChildNode in notebook)
    {
        Console.WriteLine(notebookChildNode.DisplayName);
        if (notebookChildNode is Document)
        {
            // Gör något med barndokument
        }
        else if (notebookChildNode is Notebook)
        {
            // Gör något med barnets anteckningsbok
        }
    }
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
```

### Se även

* interface [INotebookChildNode](../inotebookchildnode)
* namnutrymme [Aspose.Note](../../aspose.note)
* hopsättning [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
