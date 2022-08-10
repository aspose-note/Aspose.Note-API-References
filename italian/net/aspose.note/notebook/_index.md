---
title: Notebook
second_title: Aspose.Note per .NET API Reference
description: Rappresenta un taccuino Aspose.Note.
type: docs
weight: 390
url: /it/net/aspose.note/notebook/
---
## Notebook class

Rappresenta un taccuino Aspose.Note.

```csharp
public class Notebook : IEnumerable<INotebookChildNode>, INotebookChildNode
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Notebook](notebook#constructor)() | Inizializza una nuova istanza di[`Notebook`](../notebook) classe. |
| [Notebook](notebook#constructor_1)(Stream) | Inizializza una nuova istanza di[`Notebook`](../notebook) class. Apre un blocco appunti di OneNote esistente da uno stream. |
| [Notebook](notebook#constructor_3)(string) | Inizializza una nuova istanza di[`Notebook`](../notebook) class. Apre un blocco appunti di OneNote esistente da un file. |
| [Notebook](notebook#constructor_2)(Stream, NotebookLoadOptions) | Inizializza una nuova istanza di[`Notebook`](../notebook) class. Apre un blocco appunti di OneNote esistente da uno stream. Consente di specificare ulteriori opzioni di caricamento. |
| [Notebook](notebook#constructor_4)(string, NotebookLoadOptions) | Inizializza una nuova istanza di[`Notebook`](../notebook)class. Apre un blocco appunti di OneNote esistente da un file. Consente di specificare opzioni aggiuntive come una strategia di caricamento dei bambini ("pigro"/istantaneo). |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Color](../../aspose.note/notebook/color) { get; set; } | Ottiene o imposta il colore. |
| [Count](../../aspose.note/notebook/count) { get; } | Ottiene il numero di elementi contenuti nel file[`Notebook`](../notebook) . |
| [DisplayName](../../aspose.note/notebook/displayname) { get; set; } | Ottiene o imposta il nome visualizzato. |
| [FileFormat](../../aspose.note/notebook/fileformat) { get; } | Ottiene il formato file (OneNote 2010, OneNote Online). |
| [Guid](../../aspose.note/notebook/guid) { get; } | Ottiene l'ID univoco globale dell'oggetto. |
| [IsHistoryEnabled](../../aspose.note/notebook/ishistoryenabled) { get; set; } | Ottiene o imposta un valore che indica se la cronologia è abilitata. |
| [Item](../../aspose.note/notebook/item) { get; } | Ottiene il nodo figlio del notebook in base all'indice specificato. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AppendChild](../../aspose.note/notebook/appendchild)(INotebookChildNode) | Aggiunge il nodo alla fine dell'elenco. |
| [GetChildNodes&lt;T1&gt;](../../aspose.note/notebook/getchildnodes)() | Ottieni tutti i nodi figlio in base al tipo di nodo. |
| [GetEnumerator](../../aspose.note/notebook/getenumerator)() | Restituisce un enumeratore che scorre i nodi figlio di[`Notebook`](../notebook) . |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument)(Stream) | Aggiunge un nodo documento figlio. Apre un documento OneNote esistente da uno stream. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument_2)(string) | Aggiunge un nodo documento figlio. Apre un documento OneNote esistente da un file. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument_1)(Stream, LoadOptions) | Aggiunge un nodo documento figlio. Apre un documento OneNote esistente da uno stream. Consente di specificare ulteriori opzioni di caricamento. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument_3)(string, LoadOptions) | Aggiunge un nodo documento figlio. Apre un documento OneNote esistente da un file. Consente di specificare ulteriori opzioni di caricamento. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook)(Stream) | Aggiunge un nodo di blocco appunti figlio. Apre un blocco appunti di OneNote esistente da uno stream. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook_2)(string) | Aggiunge un nodo del blocco appunti figlio. Apre un blocco appunti di OneNote esistente da un file. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook_1)(Stream, NotebookLoadOptions) | Aggiunge un nodo del blocco appunti figlio. Apre un blocco appunti di OneNote esistente da un flusso. Consente di specificare ulteriori opzioni di caricamento. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook_3)(string, NotebookLoadOptions) | Aggiunge un nodo del blocco appunti figlio. Apre un blocco appunti di OneNote esistente da un file. Consente di specificare ulteriori opzioni di caricamento. |
| [RemoveChild](../../aspose.note/notebook/removechild)(INotebookChildNode) | Rimuove il nodo figlio. |
| [Save](../../aspose.note/notebook/save#save)(Stream) | Salva il documento di OneNote in un flusso. |
| [Save](../../aspose.note/notebook/save#save_3)(string) | Salva il documento di OneNote in un file. |
| [Save](../../aspose.note/notebook/save#save_2)(Stream, NotebookSaveOptions) | Salva il documento di OneNote in un flusso utilizzando le opzioni di salvataggio specificate. |
| [Save](../../aspose.note/notebook/save#save_1)(Stream, SaveFormat) | Salva il documento di OneNote in un flusso nel formato specificato. |
| [Save](../../aspose.note/notebook/save#save_5)(string, NotebookSaveOptions) | Salva il documento di OneNote in un file utilizzando le opzioni di salvataggio specificate. |
| [Save](../../aspose.note/notebook/save#save_4)(string, SaveFormat) | Salva il documento di OneNote in un file nel formato specificato. |

### Esempi

Mostra come salvare il taccuino.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_NoteBook();

var notebook = new Notebook();

dataDir = dataDir + "test_out.onetoc2";

// Salva il taccuino
notebook.Save(dataDir);
```

Mostra come salvare il taccuino in formato pdf.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Carica un blocco appunti di OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Salva il taccuino
notebook.Save(dataDir);
```

Mostra come salvare il taccuino come immagine.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Carica un blocco appunti di OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToImage_out.png";

// Salva il taccuino
notebook.Save(dataDir);
```

Mostra come ottenere tutto il testo da un taccuino.

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

Mostra come salvare il taccuino appiattito in formato pdf.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Carica un blocco appunti di OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Salva il taccuino
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

Mostra come scorrere i documenti di un notebook caricandoli pigramente.

```csharp
string inputFile = "Notizbuch öffnen.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

// Per impostazione predefinita, il caricamento dei bambini è "pigro".
Notebook notebook = new Notebook(dataDir + inputFile);

foreach (var notebookChildNode in notebook.OfType<Document>()) 
{
    // Il caricamento effettivo del documento figlio avviene solo qui.
    // Fai qualcosa con il documento figlio
}
```

Mostra come aggiungere una nuova sezione a un taccuino.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Carica un blocco appunti di OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Aggiunge un nuovo figlio al taccuino
notebook.AppendChild(new Document(dataDir + "Neuer Abschnitt 1.one"));

dataDir = dataDir + "AddChildNode_out.onetoc2";

// Salva il taccuino
notebook.Save(dataDir);
```

Mostra come caricare il notebook da un flusso.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

Mostra come utilizzare un notebook crittografato.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

Mostra come salvare il taccuino come immagine con le opzioni specificate.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Carica un blocco appunti di OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// Salva il taccuino
notebook.Save(dataDir, notebookSaveOptions);
```

Mostra come salvare il taccuino appiattito come immagine.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Carica un blocco appunti di OneNote
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Salva il taccuino
notebook.Save(dataDir, notebookSaveOptions);
```

Mostra come rimuovere una sezione da un blocco appunti.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Carica un blocco appunti di OneNote
var notebook = new Notebook(dataDir + "test.onetoc2");

// Attraversa i suoi nodi figlio per cercare l'elemento figlio desiderato
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // Rimuovi l'elemento figlio dal taccuino
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// Salva il taccuino
notebook.Save(dataDir);
```

Mostra come scorrere i documenti precaricati di un notebook.

```csharp
// Per impostazione predefinita, il caricamento dei bambini è "pigro".
// Pertanto per il caricamento istantaneo è avvenuto,
// è necessario impostare il flag NotebookLoadOptions.InstantLoading.
NotebookLoadOptions loadOptions = new NotebookLoadOptions { InstantLoading = true };

String inputFile = "Notizbuch öffnen.onetoc2";
String dataDir = RunExamples.GetDataDir_NoteBook();
Notebook notebook = new Notebook(dataDir + inputFile, loadOptions);

// Tutti i documenti figlio sono già caricati.
foreach (INotebookChildNode notebookChildNode in notebook.OfType<Document>()) 
{
   // Fai qualcosa con il documento figlio
}
```

Mostra come passare attraverso il contenuto di un taccuino.

```csharp
// Il percorso della directory dei documenti.
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
            // Fai qualcosa con il documento figlio
        }
        else if (notebookChildNode is Notebook)
        {
            // Fai qualcosa con il taccuino figlio
        }
    }
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
```

### Guarda anche

* interface [INotebookChildNode](../inotebookchildnode)
* spazio dei nomi [Aspose.Note](../../aspose.note)
* assemblea [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
