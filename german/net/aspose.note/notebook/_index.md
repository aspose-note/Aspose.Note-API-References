---
title: Class Notebook
second_title: Aspose.Note für .NET-API-Referenz
description: Aspose.Note.Notebook klas. Stellt ein Aspose.NoteNotizbuch dar.
type: docs
weight: 410
url: /de/net/aspose.note/notebook/
---
## Notebook class

Stellt ein Aspose.Note-Notizbuch dar.

```csharp
public class Notebook : IEnumerable<INotebookChildNode>, INotebookChildNode
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [Notebook](notebook/#constructor)() | Initialisiert eine neue Instanz von`Notebook` Klasse. |
| [Notebook](notebook/#constructor_1)(Stream) | Initialisiert eine neue Instanz von`Notebook` class. Öffnet ein vorhandenes OneNote-Notizbuch aus einem Stream. |
| [Notebook](notebook/#constructor_3)(string) | Initialisiert eine neue Instanz von`Notebook` class. Öffnet ein vorhandenes OneNote-Notizbuch aus einer Datei. |
| [Notebook](notebook/#constructor_2)(Stream, NotebookLoadOptions) | Initialisiert eine neue Instanz von`Notebook` class. Öffnet ein vorhandenes OneNote-Notizbuch aus einem Stream. Ermöglicht die Angabe zusätzlicher Ladeoptionen. |
| [Notebook](notebook/#constructor_4)(string, NotebookLoadOptions) | Initialisiert eine neue Instanz von`Notebook` class. Öffnet ein vorhandenes OneNote-Notizbuch aus einer Datei. Ermöglicht die Angabe zusätzlicher Optionen, wie z. B. eine untergeordnete Ladestrategie ("faul"/instant). |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Color](../../aspose.note/notebook/color/) { get; set; } | Ruft die Farbe ab oder legt sie fest. |
| [Count](../../aspose.note/notebook/count/) { get; } | Ruft die Anzahl der Elemente ab, die in enthalten sind`Notebook` . |
| [DisplayName](../../aspose.note/notebook/displayname/) { get; set; } | Ruft den Anzeigenamen ab oder legt ihn fest. |
| [FileFormat](../../aspose.note/notebook/fileformat/) { get; } | Ruft das Dateiformat ab (OneNote 2010, OneNote Online). |
| [Guid](../../aspose.note/notebook/guid/) { get; } | Ruft die global eindeutige ID des Objekts ab. |
| [IsHistoryEnabled](../../aspose.note/notebook/ishistoryenabled/) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob der Verlauf aktiviert ist. |
| [Item](../../aspose.note/notebook/item/) { get; } | Ruft den untergeordneten Knoten des Notebooks anhand des angegebenen Index ab. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AppendChild](../../aspose.note/notebook/appendchild/)(INotebookChildNode) | Fügt den Knoten am Ende der Liste hinzu. |
| [GetChildNodes&lt;T1&gt;](../../aspose.note/notebook/getchildnodes/)() | Alle untergeordneten Knoten nach Knotentyp abrufen. |
| [GetEnumerator](../../aspose.note/notebook/getenumerator/)() | Gibt einen Enumerator zurück, der die untergeordneten Knoten von iteriert`Notebook` . |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument)(Stream) | Fügt einen untergeordneten Dokumentknoten hinzu. Öffnet ein vorhandenes OneNote-Dokument aus einem Stream. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument_2)(string) | Fügt einen untergeordneten Dokumentknoten hinzu. Öffnet ein vorhandenes OneNote-Dokument aus einer Datei. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument_1)(Stream, LoadOptions) | Fügt einen untergeordneten Dokumentknoten hinzu. Öffnet ein vorhandenes OneNote-Dokument aus einem Stream. Ermöglicht die Angabe zusätzlicher Ladeoptionen. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument_3)(string, LoadOptions) | Fügt einen untergeordneten Dokumentknoten hinzu. Öffnet ein vorhandenes OneNote-Dokument aus einer Datei. Ermöglicht die Angabe zusätzlicher Ladeoptionen. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook)(Stream) | Fügt einen untergeordneten Notizbuchknoten hinzu. Öffnet ein vorhandenes OneNote-Notizbuch aus einem Stream. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook_2)(string) | Fügt einen untergeordneten Notizbuchknoten hinzu. Öffnet ein vorhandenes OneNote-Notizbuch aus einer Datei. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook_1)(Stream, NotebookLoadOptions) | Fügt einen untergeordneten Notizbuchknoten hinzu. Öffnet ein vorhandenes OneNote-Notizbuch aus einem Stream. Ermöglicht die Angabe zusätzlicher Ladeoptionen. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook_3)(string, NotebookLoadOptions) | Fügt einen untergeordneten Notizbuchknoten hinzu. Öffnet ein vorhandenes OneNote-Notizbuch aus einer Datei. Ermöglicht die Angabe zusätzlicher Ladeoptionen. |
| [RemoveChild](../../aspose.note/notebook/removechild/)(INotebookChildNode) | Entfernt den untergeordneten Knoten. |
| [Save](../../aspose.note/notebook/save/#save)(Stream) | Speichert das OneNote-Dokument in einem Stream. |
| [Save](../../aspose.note/notebook/save/#save_3)(string) | Speichert das OneNote-Dokument in einer Datei. |
| [Save](../../aspose.note/notebook/save/#save_2)(Stream, NotebookSaveOptions) | Speichert das OneNote-Dokument unter Verwendung der angegebenen Speicheroptionen in einem Stream. |
| [Save](../../aspose.note/notebook/save/#save_1)(Stream, SaveFormat) | Speichert das OneNote-Dokument in einem Stream im angegebenen Format. |
| [Save](../../aspose.note/notebook/save/#save_5)(string, NotebookSaveOptions) | Speichert das OneNote-Dokument unter Verwendung der angegebenen Speicheroptionen in einer Datei. |
| [Save](../../aspose.note/notebook/save/#save_4)(string, SaveFormat) | Speichert das OneNote-Dokument in einer Datei im angegebenen Format. |

### Beispiele

Zeigt, wie Notizbuch gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_NoteBook();

var notebook = new Notebook();

dataDir = dataDir + "test_out.onetoc2";

// Speichern Sie das Notizbuch
notebook.Save(dataDir);
```

Zeigt, wie Notizbücher im PDF-Format gespeichert werden.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Ein OneNote-Notizbuch laden
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Speichern Sie das Notizbuch
notebook.Save(dataDir);
```

Zeigt, wie Notizbuch als Bild gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Ein OneNote-Notizbuch laden
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToImage_out.png";

// Speichern Sie das Notizbuch
notebook.Save(dataDir);
```

Zeigt, wie der gesamte Text aus einem Notizbuch abgerufen wird.

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

Zeigt, wie ein reduziertes Notizbuch im PDF-Format gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Ein OneNote-Notizbuch laden
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Speichern Sie das Notizbuch
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

Zeigt, wie Dokumente eines Notebooks durchlaufen werden, indem sie träge geladen werden.

```csharp
string inputFile = "Notizbuch öffnen.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

// Standardmäßig ist das Laden von Kindern "faul".
Notebook notebook = new Notebook(dataDir + inputFile);

foreach (var notebookChildNode in notebook.OfType<Document>()) 
{
    // Das eigentliche Laden des untergeordneten Dokuments findet nur hier statt.
    // Etwas mit untergeordnetem Dokument tun
}
```

Zeigt, wie Sie einem Notizbuch einen neuen Abschnitt hinzufügen.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Ein OneNote-Notizbuch laden
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Ein neues untergeordnetes Element an das Notebook anhängen
notebook.AppendChild(new Document(dataDir + "Neuer Abschnitt 1.one"));

dataDir = dataDir + "AddChildNode_out.onetoc2";

// Speichern Sie das Notizbuch
notebook.Save(dataDir);
```

Zeigt, wie ein Notebook aus einem Stream geladen wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

Zeigt, wie man ein verschlüsseltes Notizbuch erstellt.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

Zeigt, wie Notizbuch als Bild mit bestimmten Optionen gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Ein OneNote-Notizbuch laden
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// Speichern Sie das Notizbuch
notebook.Save(dataDir, notebookSaveOptions);
```

Zeigt, wie ein reduziertes Notizbuch als Bild gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Ein OneNote-Notizbuch laden
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Speichern Sie das Notizbuch
notebook.Save(dataDir, notebookSaveOptions);
```

Zeigt, wie ein Abschnitt aus einem Notizbuch entfernt wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Ein OneNote-Notizbuch laden
var notebook = new Notebook(dataDir + "test.onetoc2");

// Die untergeordneten Knoten durchlaufen, um das gewünschte untergeordnete Element zu suchen
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // Entfernen Sie das untergeordnete Element aus dem Notizbuch
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// Speichern Sie das Notizbuch
notebook.Save(dataDir);
```

Zeigt, wie vorab geladene Dokumente eines Notebooks durchlaufen werden.

```csharp
// Standardmäßig ist das Laden von Kindern "faul".
// Daher hat ein sofortiges Laden stattgefunden,
// Es ist notwendig, das NotebookLoadOptions.InstantLoading-Flag zu setzen.
NotebookLoadOptions loadOptions = new NotebookLoadOptions { InstantLoading = true };

String inputFile = "Notizbuch öffnen.onetoc2";
String dataDir = RunExamples.GetDataDir_NoteBook();
Notebook notebook = new Notebook(dataDir + inputFile, loadOptions);

// Alle untergeordneten Dokumente sind bereits geladen.
foreach (INotebookChildNode notebookChildNode in notebook.OfType<Document>()) 
{
   // Etwas mit untergeordnetem Dokument tun
}
```

Zeigt, wie der Inhalt eines Notizbuchs übergeben wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
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
            // Etwas mit untergeordnetem Dokument tun
        }
        else if (notebookChildNode is Notebook)
        {
            // Mache etwas mit dem untergeordneten Notizbuch
        }
    }
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
```

### Siehe auch

* interface [INotebookChildNode](../inotebookchildnode/)
* namensraum [Aspose.Note](../../aspose.note/)
* Montage [Aspose.Note](../../)


