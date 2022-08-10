---
title: Document
second_title: Aspose.Note per .NET API Reference
description: Rappresenta un documento Aspose.Note.
type: docs
weight: 60
url: /it/net/aspose.note/document/
---
## Document class

Rappresenta un documento Aspose.Note.

```csharp
public class Document : CompositeNode<Page>, INotebookChildNode
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Document](document#constructor)() | Inizializza una nuova istanza di[`Document`](../document) class. Crea un documento OneNote vuoto. |
| [Document](document#constructor_1)(Stream) | Inizializza una nuova istanza di[`Document`](../document) class. Apre un documento OneNote esistente da uno stream. |
| [Document](document#constructor_3)(string) | Inizializza una nuova istanza di[`Document`](../document) class. Apre un documento OneNote esistente da un file. |
| [Document](document#constructor_2)(Stream, LoadOptions) | Inizializza una nuova istanza di[`Document`](../document) class. Apre un documento OneNote esistente da uno stream. Consente di specificare opzioni aggiuntive come una password di crittografia. |
| [Document](document#constructor_4)(string, LoadOptions) | Inizializza una nuova istanza di[`Document`](../document) class. Apre un documento OneNote esistente da un file. Consente di specificare opzioni aggiuntive come una password di crittografia. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AutomaticLayoutChangesDetectionEnabled](../../aspose.note/document/automaticlayoutchangesdetectionenabled) { get; set; } | Ottiene o imposta un valore che indica se Aspose.Note esegue il rilevamento automatico delle modifiche al layout. Il valore predefinito è`VERO` . |
| [Color](../../aspose.note/document/color) { get; set; } | Ottiene o imposta il colore. |
| [CreationTime](../../aspose.note/document/creationtime) { get; set; } | Ottiene o imposta l'ora di creazione. |
| [DisplayName](../../aspose.note/document/displayname) { get; set; } | Ottiene o imposta il nome visualizzato. |
| [Document](../../aspose.note/node/document) { get; } | Ottiene il documento del nodo. |
| [FileFormat](../../aspose.note/document/fileformat) { get; } | Ottiene il formato file (OneNote 2010, OneNote Online). |
| [FirstChild](../../aspose.note/compositenode`1/firstchild) { get; } |  |
| [Guid](../../aspose.note/document/guid) { get; } | Ottiene l'ID univoco globale dell'oggetto. |
| [IsComposite](../../aspose.note/compositenode`1/iscomposite) { get; } |  |
| [LastChild](../../aspose.note/compositenode`1/lastchild) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | Ottiene il nodo successivo allo stesso livello di albero dei nodi. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | Ottiene il tipo di nodo. |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | Ottiene il nodo padre. |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | Ottiene il nodo precedente allo stesso livello di albero dei nodi. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Accept](../../aspose.note/document/accept)(DocumentVisitor) | Accetta il visitatore del nodo. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildfirst)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildlast)(T1) |  |
| [DetectLayoutChanges](../../aspose.note/document/detectlayoutchanges)() | Rileva tutte le modifiche apportate al layout del documento rispetto al precedente[`DetectLayoutChanges`](./detectlayoutchanges) call. Nel caso[`AutomaticLayoutChangesDetectionEnabled`](./automaticlayoutchangesdetectionenabled) impostato su true, utilizzato automaticamente all'inizio dell'esportazione del documento. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode`1/getchildnodes)() |  |
| [GetEnumerator](../../aspose.note/compositenode`1/getenumerator)() |  |
| [GetPageHistory](../../aspose.note/document/getpagehistory)(Page) | Ottiene il[`PageHistory`](../pagehistory) che contiene la cronologia completa per ogni pagina presentata in un documento (la prima all'indice 0). È possibile accedere alla revisione della pagina corrente come[`Current`](../pagehistory/current) contenuto separatamente dalla raccolta delle versioni storiche. |
| [Import](../../aspose.note/document/import#import)(Stream, PdfImportOptions, MergeOptions) | Importa una serie di pagine dal documento PDF fornito. |
| [Import](../../aspose.note/document/import#import_1)(string, PdfImportOptions, MergeOptions) | Importa una serie di pagine dal documento PDF fornito. |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode`1/insertchild)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, IEnumerable&lt;Page&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, params Page[]) |  |
| [Merge](../../aspose.note/document/merge)(IEnumerable&lt;Page&gt;, MergeOptions) | Unisce un insieme di pagine al documento. |
| [Print](../../aspose.note/document/print#print)() | Stampa il documento utilizzando la stampante predefinita. |
| [Print](../../aspose.note/document/print#print_1)(PrintOptions) | Stampa il documento utilizzando la stampante predefinita. |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode`1/removechild)(T1) |  |
| [Save](../../aspose.note/document/save#save)(Stream) | Salva il documento di OneNote in un flusso. |
| [Save](../../aspose.note/document/save#save_3)(string) | Salva il documento di OneNote in un file. |
| [Save](../../aspose.note/document/save#save_1)(Stream, SaveFormat) | Salva il documento di OneNote in un flusso nel formato specificato. |
| [Save](../../aspose.note/document/save#save_2)(Stream, SaveOptions) | Salva il documento di OneNote in un flusso utilizzando le opzioni di salvataggio specificate. |
| [Save](../../aspose.note/document/save#save_4)(string, SaveFormat) | Salva il documento di OneNote in un file nel formato specificato. |
| [Save](../../aspose.note/document/save#save_5)(string, SaveOptions) | Salva il documento di OneNote in un file utilizzando le opzioni di salvataggio specificate. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted)(Stream, out Document) | Verifica se un documento da un flusso è crittografato. Per verificarlo dobbiamo caricare completamente questo documento. Quindi questo metodo può comportare una riduzione delle prestazioni. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_3)(string, out Document) | Verifica se un documento da un file è crittografato. Per verificarlo dobbiamo caricare completamente questo documento. Quindi questo metodo può comportare una riduzione delle prestazioni. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_1)(Stream, LoadOptions, out Document) | Verifica se un documento da un flusso è crittografato. Per verificarlo dobbiamo caricare completamente questo documento. Quindi questo metodo può comportare una riduzione delle prestazioni. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_2)(Stream, string, out Document) | Verifica se un documento da un flusso è crittografato. Per verificarlo dobbiamo caricare completamente questo documento. Quindi questo metodo può comportare una riduzione delle prestazioni. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_4)(string, LoadOptions, out Document) | Verifica se un documento da un file è crittografato. Per verificarlo dobbiamo caricare completamente questo documento. Quindi questo metodo può comportare una riduzione delle prestazioni. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_5)(string, string, out Document) | Verifica se un documento da un file è crittografato. Per verificarlo dobbiamo caricare completamente questo documento. Quindi questo metodo può comportare una riduzione delle prestazioni. |

### Esempi

Mostra come inviare un documento a una stampante utilizzando la finestra di dialogo standard di Windows con le opzioni predefinite.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
```

Mostra come salvare un documento.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

Mostra come creare un documento crittografato.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

Mostra come salvare il documento con la crittografia.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

Mostra come salvare un documento usando l'enumerazione SaveFormat.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

Mostra come salvare un documento utilizzando OneSaveOptions.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

Mostra come ottenere il conteggio delle pagine di un documento.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Pages();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Ottieni il numero di pagine
int count = oneFile.Count();

// Stampa il conteggio sulla schermata di output
Console.WriteLine(count);
```

Mostra come salvare un documento in formato pdf utilizzando le impostazioni predefinite.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Salva il documento come PDF
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Mostra come salvare un documento in formato gif.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// Salva il documento come gif.
oneFile.Save(dataDir, SaveFormat.Gif);
```

Mostra come impostare una qualità dell'immagine quando si salva un documento come immagine in formato JPEG.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Salva il documento.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

Mostra come impostare una risoluzione dell'immagine durante il salvataggio del documento come immagine.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Salva il documento.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

Mostra come ottenere il formato file di un documento.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");
switch (document.FileFormat)
{
    case FileFormat.OneNote2010:
        // Elabora OneNote 2010
        break;
    case FileFormat.OneNoteOnline:
        // Elabora OneNote in linea
        break;
}
```

Mostra come associare un collegamento ipertestuale a un'immagine.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://immagine.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

Mostra come salvare un documento in uno stream.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// Riavvolgi la posizione del flusso a zero in modo che sia pronto per il prossimo lettore.
dstStream.Seek(0, SeekOrigin.Begin);
```

Mostra come verificare se un documento è protetto da password.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
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

Mostra come verificare se il caricamento di un documento non è riuscito perché il formato OneNote 2007 non è supportato.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "OneNote2007.one");

try
{
    new Document(fileName);
}
catch (UnsupportedFileFormatException e)
{
    if (e.FileFormat == FileFormat.OneNote2007)
    {
        Console.WriteLine("It looks like the provided file is in OneNote 2007 format that is not supported.");
    }
    else
        throw;
}
```

Mostra come ripristinare la versione precedente di una pagina.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Pages();

// Carica il documento OneNote e ottieni il primo figlio           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;           
Page previousPageVersion = document.GetPageHistory(page).Last();

document.RemoveChild(page);
document.AppendChildLast(previousPageVersion);

document.Save(dataDir + "RollBackRevisions_out.one");
```

Mostra come clonare una pagina.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Pages();

// Carica il documento OneNote
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Clona in un nuovo documento senza cronologia
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// Clona in un nuovo documento con la cronologia
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

Mostra come salvare un documento in formato html con la memorizzazione di tutte le risorse (css/fonts/images) in un file separato.

```csharp
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

var options = new HtmlSaveOptions()
             {
                 ExportCss = ResourceExportType.ExportAsStream,
                 ExportFonts = ResourceExportType.ExportAsStream,
                 ExportImages = ResourceExportType.ExportAsStream,
                 FontFaceTypes = FontFaceType.Ttf
             };
document.Save(dataDir + "document_out.html", options);
```

Mostra come salvare un documento in un flusso in formato html con l'incorporamento di tutte le risorse (css/fonts/images).

```csharp
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

var options = new HtmlSaveOptions()
             {
                 ExportCss = ResourceExportType.ExportEmbedded,
                 ExportFonts = ResourceExportType.ExportEmbedded,
                 ExportImages = ResourceExportType.ExportEmbedded,
                 FontFaceTypes = FontFaceType.Ttf
             };

var r = new MemoryStream();
document.Save(r, options);
```

Mostra come impostare la descrizione del testo per un'immagine.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Images();

var document = new Document();
var page = new Page(document);
var image = new Image(document, dataDir + "image.jpg")
            {
                AlternativeTextTitle = "This is an image's title!",
                AlternativeTextDescription = "And this is an image's description!"
            };
page.AppendChildLast(image);
document.AppendChildLast(page);

dataDir = dataDir + "ImageAlternativeText_out.one";
document.Save(dataDir);
```

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

Quando le pagine lunghe di OneNote vengono salvate in formato pdf, vengono suddivise in pagine. L'esempio mostra come configurare la logica di suddivisione degli oggetti che si trovano nelle interruzioni di pagina.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// o
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

Mostra come salvare un documento in formato png.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Inizializza l'oggetto ImageSaveOptions 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // Imposta l'indice della pagina
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// Salva il documento come PNG.
oneFile.Save(dataDir, opts);
```

Mostra come modificare la cronologia della pagina.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Pages();

// Carica il documento OneNote e ottieni il primo figlio           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.RemoveRange(0, 1);

pageHistory[0] = new Page(document);
if (pageHistory.Count > 1)
{
    pageHistory[1].Title.TitleText.Text = "New Title";

    pageHistory.Add(new Page(document));

    pageHistory.Insert(1, new Page(document));

    document.Save(dataDir + "ModifyPageHistory_out.one");
}
```

Mostra come verificare se un documento è protetto da una password specifica.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
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

Mostra come ottenere un'immagine da un documento.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Images();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Ottieni tutti i nodi Immagine
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Salva i byte dell'immagine in un file
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

Mostra come salvare un documento in formato pdf.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Inizializza l'oggetto PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Imposta l'indice della prima pagina da salvare
                              PageIndex = 0,

                              // Imposta il conteggio delle pagine
                              PageCount = 1,
                          };

// Salva il documento come PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Mostra come salvare un documento in formato pdf utilizzando impostazioni specifiche.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Inizializza l'oggetto PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Usa la compressione JPEG
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Qualità per la compressione JPEG
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

Mostra come inviare un documento a una stampante utilizzando la finestra di dialogo standard di Windows con le opzioni specificate.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

var printerSettings = new PrinterSettings() { FromPage = 0, ToPage = 10 };
printerSettings.DefaultPageSettings.Landscape = true;
printerSettings.DefaultPageSettings.Margins = new System.Drawing.Printing.Margins(50, 50, 150, 50);

document.Print(new PrintOptions()
               {
                   PrinterSettings = printerSettings,
                   Resolution = 1200,
                   PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(),
                   DocumentName = "Test.one"
               });
```

Mostra come ottenere le metainformazioni dell'immagine.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Images();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Ottieni tutti i nodi Immagine
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

Mostra come ottenere il contenuto di un file allegato.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Attachments();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Sample1.one");

// Ottieni un elenco di nodi file allegati
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// Scorre tutti i nodi
foreach (AttachedFile file in nodes)
{
    // Carica il file allegato su un oggetto stream
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // Crea un file locale
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // Copia il flusso di file
            CopyStream(outputStream, fileStream);
        }
    }
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

Mostra come aggiungere un file a un documento utilizzando filepath.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Attachments();

// Crea un oggetto della classe Document
Document doc = new Document();

// Inizializza l'oggetto della classe Pagina
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inizializza l'oggetto classe Outline
Outline outline = new Outline(doc);

// Inizializza l'oggetto classe OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Inizializza oggetto classe AttachedFile
AttachedFile attachedFile = new AttachedFile(doc,  dataDir + "attachment.txt");

// Aggiungi file allegato
outlineElem.AppendChildLast(attachedFile);

// Aggiunge il nodo dell'elemento struttura
outline.AppendChildLast(outlineElem);

// Aggiungi nodo struttura
page.AppendChildLast(outline);

// Aggiungi il nodo della pagina
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileByPath_out.one";
doc.Save(dataDir);
```

Mostra come creare un documento e salvarlo in formato html utilizzando le opzioni predefinite.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Inizializza il documento OneNote
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

// Stile predefinito per tutto il testo nel documento.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// Salva in formato HTML
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

Mostra come verificare se una pagina è una pagina in conflitto (ad es. contiene modifiche che OneNote non è stato in grado di unire automaticamente).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// Carica il documento OneNote
Document doc = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

var history = doc.GetPageHistory(doc.FirstChild);
for (int i = 0; i < history.Count; i++)
{
    var historyPage = history[i];
    Console.Write("    {0}. Author: {1}, {2:dd.MM.yyyy hh.mm.ss}",
                    i,
                    historyPage.PageContentRevisionSummary.AuthorMostRecent,
                    historyPage.PageContentRevisionSummary.LastModifiedTime);
    Console.WriteLine(historyPage.IsConflictPage ? ", IsConflict: true" : string.Empty);

    // Per impostazione predefinita, le pagine di conflitto vengono semplicemente saltate durante il salvataggio.
    // Se contrassegnalo come non in conflitto, verrà salvato come al solito nella cronologia.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

Mostra come aggiungere un'immagine da un file a un documento con proprietà definite dall'utente.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Images();

// Carica il documento dallo stream.
Document doc = new Document(dataDir + "Aspose.one");

// Ottieni la prima pagina del documento.
Aspose.Note.Page page = doc.FirstChild;

// Carica un'immagine dal file.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Modifica le dimensioni dell'immagine in base alle tue esigenze (opzionale).
                              Width = 100,
                              Height = 100,

                              // Imposta la posizione dell'immagine nella pagina (opzionale).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // Imposta l'allineamento dell'immagine
                              Alignment = HorizontalAlignment.Right
                          };

// Aggiungi l'immagine alla pagina.
page.AppendChildLast(image);
```

Mostra come aggiungere un file da uno stream a un documento.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Attachments();

// Crea un oggetto della classe Document
Document doc = new Document();

// Inizializza l'oggetto della classe Pagina
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inizializza l'oggetto classe Outline
Outline outline = new Outline(doc);

// Inizializza l'oggetto classe OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // Inizializza l'oggetto classe AttachedFile e passa anche il percorso dell'icona
    AttachedFile attachedFile = new AttachedFile(doc, dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // Aggiungi file allegato
    outlineElem.AppendChildLast(attachedFile);
}

// Aggiunge il nodo dell'elemento struttura
outline.AppendChildLast(outlineElem);

// Aggiungi nodo struttura
page.AppendChildLast(outline);

// Aggiungi il nodo della pagina
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileAndSetIcon_out.one";
doc.Save(dataDir);
```

Quando le pagine lunghe di OneNote vengono salvate in formato pdf, vengono suddivise in pagine. L'esempio mostra come configurare la logica di suddivisione degli oggetti che si trovano nelle interruzioni di pagina.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// O
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// O
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// O
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// O
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

Mostra come creare un documento e salvare in formato html l'intervallo di pagine specificato.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Inizializza il documento OneNote
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Stile predefinito per tutto il testo nel documento.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// Salva in formato HTML
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

Mostra come creare un documento con una pagina intitolata.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Crea un oggetto della classe Document
Document doc = new Aspose.Note.Document();

// Inizializza l'oggetto della classe Pagina
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Stile predefinito per tutto il testo nel documento.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Imposta le proprietà del titolo della pagina
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Aggiungi il nodo Pagina nel documento
doc.AppendChildLast(page);

// Salva il documento di OneNote
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

Mostra come aggiungere un'immagine dallo stream a un documento.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Images();

// Crea un oggetto della classe Document
Document doc = new Document();

// Inizializza l'oggetto della classe Pagina
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // Carica la seconda immagine utilizzando il nome dell'immagine, l'estensione e lo stream.
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // Imposta l'allineamento dell'immagine
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// Salva il documento di OneNote
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

Mostra come aggiungere un'immagine da un file a un documento.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Images();

// Crea un oggetto della classe Document
Document doc = new Document();

// Inizializza l'oggetto della classe Pagina
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inizializza l'oggetto classe Outline e imposta le proprietà di offset
Outline outline = new Outline(doc);

// Inizializza l'oggetto classe OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Carica un'immagine dal percorso del file.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Imposta l'allineamento dell'immagine
                              Alignment = HorizontalAlignment.Right
                          };

// Aggiungi immagine
outlineElem.AppendChildLast(image);

// Aggiungi elementi di contorno
outline.AppendChildLast(outlineElem);

//Aggiungi nodo Struttura
page.AppendChildLast(outline);

// Aggiungi il nodo Pagina
doc.AppendChildLast(page);

// Salva il documento di OneNote
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

Mostra come creare un documento con un testo.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Crea un oggetto della classe Document
Document doc = new Document();

// Inizializza l'oggetto della classe Pagina
Page page = new Page(doc);

// Inizializza l'oggetto classe Outline
Outline outline = new Outline(doc);

// Inizializza l'oggetto classe OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Inizializza l'oggetto classe TextStyle e imposta le proprietà di formattazione
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Inizializza l'oggetto della classe RichText e applica lo stile del testo
RichText text = new RichText(doc) { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// Aggiunge il nodo RichText
outlineElem.AppendChildLast(text);

// Aggiunge il nodo OutlineElement
outline.AppendChildLast(outlineElem);

//Aggiungi nodo Struttura
page.AppendChildLast(outline);

// Aggiungi il nodo Pagina
doc.AppendChildLast(page);

// Salva il documento di OneNote
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
doc.Save(dataDir);
```

Mostra come salvare un documento in diversi formati.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Inizializza il nuovo documento
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// Inizializza la nuova pagina
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Stile predefinito per tutto il testo nel documento.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Aggiungi il nodo della pagina
doc.AppendChildLast(page);

// Salva il documento OneNote in diversi formati, imposta la dimensione del carattere del testo e rileva manualmente le modifiche al layout.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

Mostra come salvare un documento in formato html con la memorizzazione di tutte le risorse (css/fonts/images) utilizzando i callback definiti dall'utente.

```csharp
// Il codice seguente crea la cartella 'documentFolder' contenente document.html, la cartella 'css' con il file 'style.css', la cartella 'images' con le immagini e la cartella 'fonts' con i caratteri.
// Il file 'style.css' conterrà alla fine la seguente stringa "/* Questa riga viene aggiunta allo streaming manualmente dall'utente */"
var savingCallbacks = new UserSavingCallbacks()
                          {
                              RootFolder = "documentFolder",
                              CssFolder = "css",
                              KeepCssStreamOpened = true,
                              ImagesFolder = "images",
                              FontsFolder = "fonts"
                          };
var options = new HtmlSaveOptions
              {
                  FontFaceTypes = FontFaceType.Ttf,
                  CssSavingCallback = savingCallbacks,
                  FontSavingCallback = savingCallbacks,
                  ImageSavingCallback = savingCallbacks
              };

if (!Directory.Exists(savingCallbacks.RootFolder))
{
    Directory.CreateDirectory(savingCallbacks.RootFolder);
}

string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

using (var stream = File.Create(Path.Combine(savingCallbacks.RootFolder, "document.html")))
{
    document.Save(stream, options);
}

using (var writer = new StreamWriter(savingCallbacks.CssStream))
{
    writer.WriteLine();
    writer.WriteLine("/* This line is appended to stream manually by user */");
}
```

Mostra come associare un collegamento ipertestuale a un testo.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Tasks();

// Crea un oggetto della classe Document
Document doc = new Document();

RichText titleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append("Title!");

Outline outline = new Outline()
                      {
                          MaxWidth = 200,
                          MaxHeight = 200,
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };

TextStyle textStyleRed = new TextStyle
                             {
                                 FontColor = Color.Red,
                                 FontName = "Arial",
                                 FontSize = 10,
                             };

TextStyle textStyleHyperlink = new TextStyle
                                   {
                                       IsHyperlink = true,
                                       HyperlinkAddress = "www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// Aggiungi elementi di contorno
outline.AppendChildLast(outlineElem);

// Inizializza l'oggetto della classe Title
Title title = new Title() { TitleText = titleText };

// Inizializza l'oggetto della classe Pagina
Page page = new Note.Page() { Title = title };

//Aggiungi nodo Struttura
page.AppendChildLast(outline);

// Aggiungi il nodo Pagina
doc.AppendChildLast(page);

// Salva il documento di OneNote
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

Mostra come accedere al contenuto di un documento utilizzando il visitatore.

```csharp
public static void Run()
{
    // Il percorso della directory dei documenti.
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // Apri il documento che vogliamo convertire.
    Document doc = new Document(dataDir + "Aspose.one");

    // Crea un oggetto che eredita dalla classe DocumentVisitor.
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // Questo è il noto modello Visitor. Ottieni il modello per accettare un visitatore.
    // Il modello eseguirà un'iterazione su se stesso chiamando i metodi corrispondenti
    // sull'oggetto visitatore (questo è chiamato visita).
    //
    // Nota che ogni nodo nel modello a oggetti ha il metodo Accept, quindi la visita
    // può essere eseguito non solo per l'intero documento, ma per qualsiasi nodo nel documento.
    doc.Accept(myConverter);

    // Una volta completata la visita, possiamo recuperare il risultato dell'operazione,
    // che in questo esempio si è accumulato nel visitatore.
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// Semplice implementazione del salvataggio di un documento in formato testo normale. Implementato come visitatore.
/// </summary>
public class MyOneNoteToTxtWriter : DocumentVisitor
{
    public MyOneNoteToTxtWriter()
    {
        nodecount = 0;
        mIsSkipText = false;
        mBuilder = new StringBuilder();
    }

    /// <summary>
    /// Ottiene il testo normale del documento accumulato dal visitatore.
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// Aggiunge testo all'output corrente. Rispetta il flag di uscita abilitato/disabilitato.
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// Chiamato quando viene rilevato un nodo RichText nel documento.
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// Chiamato quando viene rilevato un nodo Document nel documento.
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// Chiamato quando viene rilevato un nodo Pagina nel documento.
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// Chiamato quando l'elaborazione di un nodo Pagina è terminata.
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// Chiamato quando viene rilevato un nodo Titolo nel documento.
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// Chiamato quando viene rilevato un nodo Immagine nel documento.
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// Chiamato quando viene rilevato un nodo OutlineGroup nel documento.
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// Chiamato quando viene rilevato un nodo Struttura nel documento.
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// Chiamato quando viene rilevato un nodo OutlineElement nel documento.
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// Ottiene il conteggio totale dei nodi dal Visitatore
    /// </summary>
    public Int32 NodeCount
    {
        get { return this.nodecount; }
    }

    private readonly StringBuilder mBuilder;
    private bool mIsSkipText;
    private Int32 nodecount;
}
```

### Guarda anche

* class [CompositeNode&lt;T&gt;](../compositenode-1)
* class [Page](../page)
* interface [INotebookChildNode](../inotebookchildnode)
* spazio dei nomi [Aspose.Note](../../aspose.note)
* assemblea [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
