---
title: Class Notebook
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.Notebook klas. Vertegenwoordigt een Aspose.Notenotebook.
type: docs
weight: 410
url: /nl/net/aspose.note/notebook/
---
## Notebook class

Vertegenwoordigt een Aspose.Note-notebook.

```csharp
public class Notebook : IEnumerable<INotebookChildNode>, INotebookChildNode
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [Notebook](notebook/#constructor)() | Initialiseert een nieuw exemplaar van het`Notebook` klasse. |
| [Notebook](notebook/#constructor_1)(Stream) | Initialiseert een nieuw exemplaar van het`Notebook` class. Opent een bestaand OneNote-notitieblok vanuit een stream. |
| [Notebook](notebook/#constructor_3)(string) | Initialiseert een nieuw exemplaar van het`Notebook` class. Opent een bestaand OneNote-notitieblok vanuit een bestand. |
| [Notebook](notebook/#constructor_2)(Stream, NotebookLoadOptions) | Initialiseert een nieuw exemplaar van het`Notebook` class. Opent een bestaand OneNote-notitieblok vanuit een stream. Maakt het mogelijk om extra laadopties te specificeren. |
| [Notebook](notebook/#constructor_4)(string, NotebookLoadOptions) | Initialiseert een nieuw exemplaar van het`Notebook` class. Opent een bestaand OneNote-notitieblok vanuit een bestand. Maakt het mogelijk om extra opties te specificeren, zoals een laadstrategie voor kinderen ("lazy"/instant). |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Color](../../aspose.note/notebook/color/) { get; set; } | Krijgt of stelt de kleur in. |
| [Count](../../aspose.note/notebook/count/) { get; } | Krijgt het aantal elementen in de`Notebook` . |
| [DisplayName](../../aspose.note/notebook/displayname/) { get; set; } | Haalt de weergavenaam op of stelt deze in. |
| [FileFormat](../../aspose.note/notebook/fileformat/) { get; } | Krijgt bestandsindeling (OneNote 2010, OneNote Online). |
| [Guid](../../aspose.note/notebook/guid/) { get; } | Haalt de wereldwijd unieke id van het object op. |
| [IsHistoryEnabled](../../aspose.note/notebook/ishistoryenabled/) { get; set; } | Haalt of stelt een waarde in die aangeeft of de geschiedenis is ingeschakeld. |
| [Item](../../aspose.note/notebook/item/) { get; } | Haalt het onderliggende knooppunt van de notebook op met de gegeven index. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| [AppendChild](../../aspose.note/notebook/appendchild/)(INotebookChildNode) | Voegt het knooppunt toe aan het einde van de lijst. |
| [GetChildNodes&lt;T1&gt;](../../aspose.note/notebook/getchildnodes/)() | Alle onderliggende knooppunten ophalen op basis van het knooppunttype. |
| [GetEnumerator](../../aspose.note/notebook/getenumerator/)() | Retourneert een teller die itereert door onderliggende knooppunten van het`Notebook` . |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument)(Stream) | Voegt een onderliggend documentknooppunt toe. Opent een bestaand OneNote-document uit een stream. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument_2)(string) | Voegt een onderliggend documentknooppunt toe. Opent een bestaand OneNote-document vanuit een bestand. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument_1)(Stream, LoadOptions) | Voegt een onderliggend documentknooppunt toe. Opent een bestaand OneNote-document uit een stroom. Maakt het mogelijk om extra laadopties te specificeren. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument_3)(string, LoadOptions) | Voegt een onderliggend documentknooppunt toe. Opent een bestaand OneNote-document vanuit een bestand. Maakt het mogelijk om extra laadopties te specificeren. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook)(Stream) | Voegt een onderliggend notitieblokknooppunt toe. Opent een bestaand OneNote-notitieblok vanuit een stream. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook_2)(string) | Voegt een onderliggend notitieboekknooppunt toe. Opent een bestaand OneNote-notitieblok vanuit een bestand. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook_1)(Stream, NotebookLoadOptions) | Voegt een onderliggend notitieblokknooppunt toe. Opent een bestaand OneNote-notitieblok vanuit een stream. Maakt het mogelijk om extra laadopties te specificeren. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook_3)(string, NotebookLoadOptions) | Voegt een onderliggend notitieblokknooppunt toe. Opent een bestaand OneNote-notitieblok vanuit een bestand. Maakt het mogelijk om extra laadopties te specificeren. |
| [RemoveChild](../../aspose.note/notebook/removechild/)(INotebookChildNode) | Verwijdert het onderliggende knooppunt. |
| [Save](../../aspose.note/notebook/save/#save)(Stream) | Slaat het OneNote-document op in een stream. |
| [Save](../../aspose.note/notebook/save/#save_3)(string) | Slaat het OneNote-document op in een bestand. |
| [Save](../../aspose.note/notebook/save/#save_2)(Stream, NotebookSaveOptions) | Slaat het OneNote-document op in een stream met behulp van de opgegeven opslagopties. |
| [Save](../../aspose.note/notebook/save/#save_1)(Stream, SaveFormat) | Slaat het OneNote-document op in een stream in de opgegeven indeling. |
| [Save](../../aspose.note/notebook/save/#save_5)(string, NotebookSaveOptions) | Slaat het OneNote-document op in een bestand met de opgegeven opslagopties. |
| [Save](../../aspose.note/notebook/save/#save_4)(string, SaveFormat) | Slaat het OneNote-document op in een bestand in de opgegeven indeling. |

### Voorbeelden

Laat zien hoe u een notebook kunt opslaan.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_NoteBook();

var notebook = new Notebook();

dataDir = dataDir + "test_out.onetoc2";

// Sla het notitieblok op
notebook.Save(dataDir);
```

Laat zien hoe je een notitieboek opslaat in pdf-formaat.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Laad een OneNote-notitieblok
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Sla het notitieblok op
notebook.Save(dataDir);
```

Laat zien hoe je een notitieboek opslaat als afbeelding.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Laad een OneNote-notitieblok
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToImage_out.png";

// Sla het notitieblok op
notebook.Save(dataDir);
```

Laat zien hoe u alle tekst uit een notitieblok haalt.

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

Laat zien hoe u een afgeplat notitieboek in pdf-formaat kunt opslaan.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Laad een OneNote-notitieblok
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Sla het notitieblok op
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

Laat zien hoe u door documenten van een notebook kunt bladeren die ze lui laden.

```csharp
string inputFile = "Notizbuch öffnen.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

// Standaard is het laden van kinderen "lui".
Notebook notebook = new Notebook(dataDir + inputFile);

foreach (var notebookChildNode in notebook.OfType<Document>()) 
{
    // Alleen hier wordt het onderliggende document daadwerkelijk geladen.
    // Doe iets met het onderliggende document
}
```

Laat zien hoe je een nieuwe sectie toevoegt aan een notitieblok.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Laad een OneNote-notitieblok
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Voeg een nieuw kind toe aan de Notebook
notebook.AppendChild(new Document(dataDir + "Neuer Abschnitt 1.one"));

dataDir = dataDir + "AddChildNode_out.onetoc2";

// Sla het notitieblok op
notebook.Save(dataDir);
```

Laat zien hoe je een notebook laadt vanuit een stream.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
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

Laat zien hoe u een notitieblok kunt opslaan als afbeelding met opgegeven opties.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Laad een OneNote-notitieblok
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// Sla het notitieblok op
notebook.Save(dataDir, notebookSaveOptions);
```

Laat zien hoe u een afgeplat notitieboek als afbeelding kunt opslaan.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Laad een OneNote-notitieblok
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Sla het notitieblok op
notebook.Save(dataDir, notebookSaveOptions);
```

Laat zien hoe u een sectie uit een notitieblok verwijdert.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Laad een OneNote-notitieblok
var notebook = new Notebook(dataDir + "test.onetoc2");

// Blader door de onderliggende knooppunten om het gewenste onderliggende item te zoeken
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // Verwijder het onderliggende item uit het notitieblok
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// Sla het notitieblok op
notebook.Save(dataDir);
```

Laat zien hoe u door vooraf geladen documenten van een notebook kunt bladeren.

```csharp
// Standaard is het laden van kinderen "lui".
// Daarom heeft voor direct laden plaatsgevonden,
// het is noodzakelijk om de vlag NotebookLoadOptions.InstantLoading in te stellen.
NotebookLoadOptions loadOptions = new NotebookLoadOptions { InstantLoading = true };

String inputFile = "Notizbuch öffnen.onetoc2";
String dataDir = RunExamples.GetDataDir_NoteBook();
Notebook notebook = new Notebook(dataDir + inputFile, loadOptions);

// Alle onderliggende documenten zijn al geladen.
foreach (INotebookChildNode notebookChildNode in notebook.OfType<Document>()) 
{
   // Doe iets met het onderliggende document
}
```

Laat zien hoe u de inhoud van een notitieblok doorgeeft.

```csharp
// Het pad naar de documentenmap.
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
            // Doe iets met het onderliggende document
        }
        else if (notebookChildNode is Notebook)
        {
            // Doe iets met een kindernotitieboekje
        }
    }
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
```

### Zie ook

* interface [INotebookChildNode](../inotebookchildnode/)
* naamruimte [Aspose.Note](../../aspose.note/)
* montage [Aspose.Note](../../)


