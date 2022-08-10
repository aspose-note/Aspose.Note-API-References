---
title: Document
second_title: Aspose.Note für .NET-API-Referenz
description: Stellt ein Aspose.Note-Dokument dar.
type: docs
weight: 60
url: /de/net/aspose.note/document/
---
## Document class

Stellt ein Aspose.Note-Dokument dar.

```csharp
public class Document : CompositeNode<Page>, INotebookChildNode
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [Document](document#constructor)() | Initialisiert eine neue Instanz von[`Document`](../document) class. Erstellt ein leeres OneNote-Dokument. |
| [Document](document#constructor_1)(Stream) | Initialisiert eine neue Instanz von[`Document`](../document) class. Öffnet ein vorhandenes OneNote-Dokument aus einem Stream. |
| [Document](document#constructor_3)(string) | Initialisiert eine neue Instanz von[`Document`](../document) class. Öffnet ein vorhandenes OneNote-Dokument aus einer Datei. |
| [Document](document#constructor_2)(Stream, LoadOptions) | Initialisiert eine neue Instanz von[`Document`](../document) class. Öffnet ein vorhandenes OneNote-Dokument aus einem Stream. Ermöglicht die Angabe zusätzlicher Optionen wie z. B. eines Verschlüsselungskennworts. |
| [Document](document#constructor_4)(string, LoadOptions) | Initialisiert eine neue Instanz von[`Document`](../document) class. Öffnet ein vorhandenes OneNote-Dokument aus einer Datei. Ermöglicht die Angabe zusätzlicher Optionen wie z. B. eines Verschlüsselungskennworts. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AutomaticLayoutChangesDetectionEnabled](../../aspose.note/document/automaticlayoutchangesdetectionenabled) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob Aspose.Note die Erkennung von Layoutänderungen automatisch durchführt. Der Standardwert ist`Stimmt` . |
| [Color](../../aspose.note/document/color) { get; set; } | Ruft die Farbe ab oder legt sie fest. |
| [CreationTime](../../aspose.note/document/creationtime) { get; set; } | Ruft die Erstellungszeit ab oder legt sie fest. |
| [DisplayName](../../aspose.note/document/displayname) { get; set; } | Ruft den Anzeigenamen ab oder legt ihn fest. |
| [Document](../../aspose.note/node/document) { get; } | Ruft das Dokument des Knotens ab. |
| [FileFormat](../../aspose.note/document/fileformat) { get; } | Ruft das Dateiformat ab (OneNote 2010, OneNote Online). |
| [FirstChild](../../aspose.note/compositenode`1/firstchild) { get; } |  |
| [Guid](../../aspose.note/document/guid) { get; } | Ruft die global eindeutige ID des Objekts ab. |
| [IsComposite](../../aspose.note/compositenode`1/iscomposite) { get; } |  |
| [LastChild](../../aspose.note/compositenode`1/lastchild) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | Ruft den nächsten Knoten auf derselben Knotenbaumebene ab. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | Ruft den Knotentyp ab. |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | Ruft den übergeordneten Knoten ab. |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | Ruft den vorherigen Knoten auf derselben Knotenbaumebene ab. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [Accept](../../aspose.note/document/accept)(DocumentVisitor) | Akzeptiert den Besucher des Knotens. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildfirst)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildlast)(T1) |  |
| [DetectLayoutChanges](../../aspose.note/document/detectlayoutchanges)() | Erkennt alle Änderungen, die seit dem vorherigen am Dokumentlayout vorgenommen wurden[`DetectLayoutChanges`](./detectlayoutchanges) call. Falls[`AutomaticLayoutChangesDetectionEnabled`](./automaticlayoutchangesdetectionenabled) auf true gesetzt, wird automatisch zu Beginn des Dokumentexports verwendet. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode`1/getchildnodes)() |  |
| [GetEnumerator](../../aspose.note/compositenode`1/getenumerator)() |  |
| [GetPageHistory](../../aspose.note/document/getpagehistory)(Page) | Ruft die ab[`PageHistory`](../pagehistory) die den vollständigen Verlauf für jede Seite enthält, die in einem Dokument präsentiert wird (die früheste bei Index 0). Auf die aktuelle Seitenrevision kann zugegriffen werden als[`Current`](../pagehistory/current)und getrennt von der Sammlung historischer Versionen enthalten. |
| [Import](../../aspose.note/document/import#import)(Stream, PdfImportOptions, MergeOptions) | Importiert eine Reihe von Seiten aus dem bereitgestellten PDF-Dokument. |
| [Import](../../aspose.note/document/import#import_1)(string, PdfImportOptions, MergeOptions) | Importiert eine Reihe von Seiten aus dem bereitgestellten PDF-Dokument. |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode`1/insertchild)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, IEnumerable&lt;Page&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, params Page[]) |  |
| [Merge](../../aspose.note/document/merge)(IEnumerable&lt;Page&gt;, MergeOptions) | Führt eine Reihe von Seiten mit dem Dokument zusammen. |
| [Print](../../aspose.note/document/print#print)() | Druckt das Dokument mit dem Standarddrucker. |
| [Print](../../aspose.note/document/print#print_1)(PrintOptions) | Druckt das Dokument mit dem Standarddrucker. |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode`1/removechild)(T1) |  |
| [Save](../../aspose.note/document/save#save)(Stream) | Speichert das OneNote-Dokument in einem Stream. |
| [Save](../../aspose.note/document/save#save_3)(string) | Speichert das OneNote-Dokument in einer Datei. |
| [Save](../../aspose.note/document/save#save_1)(Stream, SaveFormat) | Speichert das OneNote-Dokument in einem Stream im angegebenen Format. |
| [Save](../../aspose.note/document/save#save_2)(Stream, SaveOptions) | Speichert das OneNote-Dokument unter Verwendung der angegebenen Speicheroptionen in einem Stream. |
| [Save](../../aspose.note/document/save#save_4)(string, SaveFormat) | Speichert das OneNote-Dokument in einer Datei im angegebenen Format. |
| [Save](../../aspose.note/document/save#save_5)(string, SaveOptions) | Speichert das OneNote-Dokument unter Verwendung der angegebenen Speicheroptionen in einer Datei. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted)(Stream, out Document) | Überprüft, ob ein Dokument aus einem Stream verschlüsselt ist. Um dies zu überprüfen, müssen wir dieses Dokument vollständig laden. Diese Methode kann also zu Leistungseinbußen führen. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_3)(string, out Document) | Überprüft, ob ein Dokument aus einer Datei verschlüsselt ist. Um dies zu überprüfen, müssen wir dieses Dokument vollständig laden. Diese Methode kann also zu Leistungseinbußen führen. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_1)(Stream, LoadOptions, out Document) | Überprüft, ob ein Dokument aus einem Stream verschlüsselt ist. Um dies zu überprüfen, müssen wir dieses Dokument vollständig laden. Diese Methode kann also zu Leistungseinbußen führen. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_2)(Stream, string, out Document) | Überprüft, ob ein Dokument aus einem Stream verschlüsselt ist. Um dies zu überprüfen, müssen wir dieses Dokument vollständig laden. Diese Methode kann also zu Leistungseinbußen führen. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_4)(string, LoadOptions, out Document) | Überprüft, ob ein Dokument aus einer Datei verschlüsselt ist. Um dies zu überprüfen, müssen wir dieses Dokument vollständig laden. Diese Methode kann also zu Leistungseinbußen führen. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_5)(string, string, out Document) | Überprüft, ob ein Dokument aus einer Datei verschlüsselt ist. Um dies zu überprüfen, müssen wir dieses Dokument vollständig laden. Diese Methode kann also zu Leistungseinbußen führen. |

### Beispiele

Zeigt, wie ein Dokument mithilfe des Standard-Windows-Dialogfelds mit Standardoptionen an einen Drucker gesendet wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
```

Zeigt, wie ein Dokument gespeichert wird.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

Zeigt, wie man ein verschlüsseltes Dokument erstellt.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

Zeigt, wie Dokumente verschlüsselt gespeichert werden.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

Zeigt, wie ein Dokument mithilfe der SaveFormat-Enumeration gespeichert wird.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

Zeigt, wie ein Dokument mit OneSaveOptions gespeichert wird.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

Zeigt, wie man die Seitenanzahl eines Dokuments erhält.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Pages();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Seitenzahl abrufen
int count = oneFile.Count();

// Anzahl auf dem Ausgabebildschirm drucken
Console.WriteLine(count);
```

Zeigt, wie Sie ein Dokument im PDF-Format mit Standardeinstellungen speichern.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Dokument als PDF speichern
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Zeigt, wie ein Dokument im gif-Format gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// Speichern Sie das Dokument als gif.
oneFile.Save(dataDir, SaveFormat.Gif);
```

Zeigt, wie eine Bildqualität eingestellt wird, wenn ein Dokument als Bild im JPEG-Format gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Speichern Sie das Dokument.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

Zeigt, wie eine Bildauflösung eingestellt wird, wenn ein Dokument als Bild gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Speichern Sie das Dokument.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

Zeigt, wie man das Dateiformat eines Dokuments erhält.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");
switch (document.FileFormat)
{
    case FileFormat.OneNote2010:
        // OneNote 2010 verarbeiten
        break;
    case FileFormat.OneNoteOnline:
        // OneNote online verarbeiten
        break;
}
```

Zeigt, wie ein Hyperlink an ein Bild gebunden wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://image.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

Zeigt, wie ein Dokument in einem Stream gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// Spulen Sie die Stream-Position auf Null zurück, damit sie für den nächsten Reader bereit ist.
dstStream.Seek(0, SeekOrigin.Begin);
```

Zeigt, wie überprüft wird, ob ein Dokument passwortgeschützt ist.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
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

Zeigt, wie überprüft wird, ob das Laden eines Dokuments fehlgeschlagen ist, weil das OneNote 2007-Format nicht unterstützt wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
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

Zeigt, wie die vorherige Version einer Seite wiederhergestellt wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote-Dokument laden und erstes untergeordnetes Element abrufen           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;           
Page previousPageVersion = document.GetPageHistory(page).Last();

document.RemoveChild(page);
document.AppendChildLast(previousPageVersion);

document.Save(dataDir + "RollBackRevisions_out.one");
```

Zeigt, wie eine Seite geklont wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote-Dokument laden
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// In neues Dokument ohne Historie klonen
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// In neues Dokument mit Verlauf klonen
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

Zeigt, wie ein Dokument im HTML-Format gespeichert wird, wobei alle Ressourcen (css/fonts/images) in separaten Dateien gespeichert werden.

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

Zeigt, wie ein Dokument in einem Stream im HTML-Format mit Einbettung aller Ressourcen (css/fonts/images) gespeichert wird.

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

Zeigt, wie eine Textbeschreibung für ein Bild festgelegt wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
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

Zeigt, wie Metainformationen zu einer Seite abgerufen werden.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Pages();

// Laden Sie das Dokument in Aspose.Note.
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

Wenn lange OneNote-Seiten im PDF-Format gespeichert werden, werden sie auf Seiten aufgeteilt. Das Beispiel zeigt, wie die Aufteilungslogik von Objekten konfiguriert wird, die sich auf Seitenumbrüchen befinden.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// oder
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

Zeigt, wie ein Dokument im PNG-Format gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// ImageSaveOptions-Objekt initialisieren 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // Seitenindex setzen
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// Speichern Sie das Dokument als PNG.
oneFile.Save(dataDir, opts);
```

Zeigt, wie der Seitenverlauf bearbeitet wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote-Dokument laden und erstes untergeordnetes Element abrufen           
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

Zeigt, wie überprüft werden kann, ob ein Dokument durch ein bestimmtes Passwort passwortgeschützt ist.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
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

Zeigt, wie ein Bild aus einem Dokument abgerufen wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Images();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Alle Image-Knoten abrufen
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Bildbytes in einer Datei speichern
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

Zeigt, wie ein Dokument im PDF-Format gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// PdfSaveOptions-Objekt initialisieren
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Seitenindex der ersten zu speichernden Seite setzen
                              PageIndex = 0,

                              // Seitenanzahl festlegen
                              PageCount = 1,
                          };

// Dokument als PDF speichern
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Zeigt, wie Sie ein Dokument im PDF-Format mit bestimmten Einstellungen speichern.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// PdfSaveOptions-Objekt initialisieren
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // JPEG-Komprimierung verwenden
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Qualität für JPEG-Komprimierung
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

Zeigt, wie ein Dokument mithilfe des Windows-Standarddialogs mit festgelegten Optionen an einen Drucker gesendet wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
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

Zeigt, wie die Metainformationen des Bildes abgerufen werden.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Images();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Alle Image-Knoten abrufen
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

Zeigt, wie der Inhalt einer angehängten Datei abgerufen wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Attachments();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Sample1.one");

// Holen Sie sich eine Liste der angehängten Dateiknoten
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// Durch alle Knoten iterieren
foreach (AttachedFile file in nodes)
{
    // Angehängte Datei in ein Stream-Objekt laden
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // Erstellen Sie eine lokale Datei
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // Dateistrom kopieren
            CopyStream(outputStream, fileStream);
        }
    }
}
```

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

Zeigt, wie Sie mithilfe von filepath eine Datei zu einem Dokument hinzufügen.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Attachments();

// Erstellen Sie ein Objekt der Document-Klasse
Document doc = new Document();

// Seitenklassenobjekt initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline-Klassenobjekt initialisieren
Outline outline = new Outline(doc);

// OutlineElement-Klassenobjekt initialisieren
OutlineElement outlineElem = new OutlineElement(doc);

// AttachedFile-Klassenobjekt initialisieren
AttachedFile attachedFile = new AttachedFile(doc,  dataDir + "attachment.txt");

// Angehängte Datei hinzufügen
outlineElem.AppendChildLast(attachedFile);

// Gliederungselementknoten hinzufügen
outline.AppendChildLast(outlineElem);

// Gliederungsknoten hinzufügen
page.AppendChildLast(outline);

// Seitenknoten hinzufügen
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileByPath_out.one";
doc.Save(dataDir);
```

Zeigt, wie Sie ein Dokument erstellen und es mit Standardoptionen im HTML-Format speichern.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// OneNote-Dokument initialisieren
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

// Standardstil für den gesamten Text im Dokument.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// Im HTML-Format speichern
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

Zeigt, wie überprüft wird, ob es sich bei einer Seite um eine Konfliktseite handelt (d. h. sie enthält Änderungen, die OneNote nicht automatisch zusammenführen konnte).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote-Dokument laden
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

    // Standardmäßig werden Konfliktseiten beim Speichern einfach übersprungen.
    // Wenn es als Nicht-Konflikt markiert wird, wird es wie gewohnt im Verlauf gespeichert.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

Zeigt, wie ein Bild aus einer Datei zu einem Dokument mit benutzerdefinierten Eigenschaften hinzugefügt wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Images();

// Dokument aus dem Stream laden.
Document doc = new Document(dataDir + "Aspose.one");

// Holen Sie sich die erste Seite des Dokuments.
Aspose.Note.Page page = doc.FirstChild;

// Laden Sie ein Bild aus der Datei.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Ändern Sie die Größe des Bildes nach Ihren Bedürfnissen (optional).
                              Width = 100,
                              Height = 100,

                              // Legen Sie die Position des Bildes auf der Seite fest (optional).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // Bildausrichtung festlegen
                              Alignment = HorizontalAlignment.Right
                          };

// Bild zur Seite hinzufügen.
page.AppendChildLast(image);
```

Zeigt, wie eine Datei aus einem Stream zu einem Dokument hinzugefügt wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Attachments();

// Erstellen Sie ein Objekt der Document-Klasse
Document doc = new Document();

// Seitenklassenobjekt initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline-Klassenobjekt initialisieren
Outline outline = new Outline(doc);

// OutlineElement-Klassenobjekt initialisieren
OutlineElement outlineElem = new OutlineElement(doc);

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // Objekt der AttachedFile-Klasse initialisieren und auch seinen Icon-Pfad übergeben
    AttachedFile attachedFile = new AttachedFile(doc, dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // Angehängte Datei hinzufügen
    outlineElem.AppendChildLast(attachedFile);
}

// Gliederungselementknoten hinzufügen
outline.AppendChildLast(outlineElem);

// Gliederungsknoten hinzufügen
page.AppendChildLast(outline);

// Seitenknoten hinzufügen
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileAndSetIcon_out.one";
doc.Save(dataDir);
```

Wenn lange OneNote-Seiten im PDF-Format gespeichert werden, werden sie auf Seiten aufgeteilt. Das Beispiel zeigt, wie die Aufteilungslogik von Objekten konfiguriert wird, die sich auf Seitenumbrüchen befinden.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// Oder
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// Oder
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// Oder
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// Oder
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

Zeigt, wie man ein Dokument erstellt und einen bestimmten Seitenbereich im HTML-Format speichert.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// OneNote-Dokument initialisieren
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Standardstil für den gesamten Text im Dokument.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// Im HTML-Format speichern
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

Zeigt, wie ein Dokument mit Titelseite erstellt wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Erstellen Sie ein Objekt der Document-Klasse
Document doc = new Aspose.Note.Document();

// Seitenklassenobjekt initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Standardstil für den gesamten Text im Dokument.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Eigenschaften des Seitentitels festlegen
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Seitenknoten im Dokument anhängen
doc.AppendChildLast(page);

// OneNote-Dokument speichern
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

Zeigt, wie ein Bild aus einem Stream zu einem Dokument hinzugefügt wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Images();

// Erstellen Sie ein Objekt der Document-Klasse
Document doc = new Document();

// Seitenklassenobjekt initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // Laden Sie das zweite Bild unter Verwendung des Bildnamens, der Erweiterung und des Streams.
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // Bildausrichtung festlegen
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// OneNote-Dokument speichern
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

Zeigt, wie Sie einem Dokument ein Bild aus einer Datei hinzufügen.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Images();

// Erstellen Sie ein Objekt der Document-Klasse
Document doc = new Document();

// Seitenklassenobjekt initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline-Klassenobjekt initialisieren und Offset-Eigenschaften festlegen
Outline outline = new Outline(doc);

// OutlineElement-Klassenobjekt initialisieren
OutlineElement outlineElem = new OutlineElement(doc);

// Laden Sie ein Bild über den Dateipfad.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Bildausrichtung festlegen
                              Alignment = HorizontalAlignment.Right
                          };

// Bild hinzufügen
outlineElem.AppendChildLast(image);

// Gliederungselemente hinzufügen
outline.AppendChildLast(outlineElem);

// Outline-Knoten hinzufügen
page.AppendChildLast(outline);

// Seitenknoten hinzufügen
doc.AppendChildLast(page);

// OneNote-Dokument speichern
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

Zeigt, wie ein Dokument mit einem Text erstellt wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Erstellen Sie ein Objekt der Document-Klasse
Document doc = new Document();

// Seitenklassenobjekt initialisieren
Page page = new Page(doc);

// Outline-Klassenobjekt initialisieren
Outline outline = new Outline(doc);

// OutlineElement-Klassenobjekt initialisieren
OutlineElement outlineElem = new OutlineElement(doc);

// TextStyle-Klassenobjekt initialisieren und Formatierungseigenschaften festlegen
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// RichText-Klassenobjekt initialisieren und Textstil anwenden
RichText text = new RichText(doc) { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// RichText-Knoten hinzufügen
outlineElem.AppendChildLast(text);

// OutlineElement-Knoten hinzufügen
outline.AppendChildLast(outlineElem);

// Outline-Knoten hinzufügen
page.AppendChildLast(outline);

// Seitenknoten hinzufügen
doc.AppendChildLast(page);

// OneNote-Dokument speichern
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
doc.Save(dataDir);
```

Zeigt, wie ein Dokument in verschiedenen Formaten gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Das neue Dokument initialisieren
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// Neue Seite initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Standardstil für den gesamten Text im Dokument.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Seitenknoten anhängen
doc.AppendChildLast(page);

// OneNote-Dokument in verschiedenen Formaten speichern, Textschriftgröße festlegen und Layoutänderungen manuell erkennen.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

Zeigt, wie ein Dokument im HTML-Format gespeichert wird, wobei alle Ressourcen (css/fonts/images) mithilfe von benutzerdefinierten Rückrufen gespeichert werden.

```csharp
// Der folgende Code erstellt den Ordner „documentFolder“ mit document.html, den Ordner „css“ mit der Datei „style.css“, den Ordner „images“ mit Bildern und den Ordner „fonts“ mit Schriftarten.
// Die Datei „style.css“ enthält am Ende die folgende Zeichenfolge „/* Diese Zeile wird vom Benutzer manuell an den Stream angehängt */“
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

Zeigt, wie ein Hyperlink an einen Text gebunden wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Tasks();

// Erstellen Sie ein Objekt der Document-Klasse
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

// Gliederungselemente hinzufügen
outline.AppendChildLast(outlineElem);

// Titelklassenobjekt initialisieren
Title title = new Title() { TitleText = titleText };

// Seitenklassenobjekt initialisieren
Page page = new Note.Page() { Title = title };

// Outline-Knoten hinzufügen
page.AppendChildLast(outline);

// Seitenknoten hinzufügen
doc.AppendChildLast(page);

// OneNote-Dokument speichern
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

Zeigt, wie Sie mit „Besucher“ auf den Inhalt eines Dokuments zugreifen.

```csharp
public static void Run()
{
    // Der Pfad zum Dokumentenverzeichnis.
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // Öffnen Sie das Dokument, das wir konvertieren möchten.
    Document doc = new Document(dataDir + "Aspose.one");

    // Ein Objekt erstellen, das von der DocumentVisitor-Klasse erbt.
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // Dies ist das bekannte Besuchermuster. Bringen Sie das Modell dazu, einen Besucher anzunehmen.
    // Das Modell iteriert durch sich selbst, indem es die entsprechenden Methoden aufruft
    // auf dem Besucherobjekt (dies wird Besuch genannt).
    //
    // Beachten Sie, dass jeder Knoten im Objektmodell die Accept-Methode hat, also den Besuch
    // kann nicht nur für das gesamte Dokument ausgeführt werden, sondern für jeden Knoten im Dokument.
    doc.Accept(myConverter);

    // Sobald der Besuch abgeschlossen ist, können wir das Ergebnis der Operation abrufen,
    // die sich in diesem Beispiel im Besucher angesammelt hat.
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// Einfache Implementierung zum Speichern eines Dokuments im Nur-Text-Format. Als Besucher implementiert.
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
    /// Ruft den Klartext des Dokuments ab, das vom Besucher angesammelt wurde.
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// Fügt Text zur aktuellen Ausgabe hinzu. Berücksichtigt das aktivierte/deaktivierte Ausgangsflag.
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// Wird aufgerufen, wenn im Dokument ein RichText-Knoten gefunden wird.
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// Wird aufgerufen, wenn im Dokument ein Dokumentknoten gefunden wird.
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// Wird aufgerufen, wenn im Dokument ein Page-Knoten gefunden wird.
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// Wird aufgerufen, wenn die Verarbeitung eines Seitenknotens abgeschlossen ist.
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// Wird aufgerufen, wenn im Dokument ein Titelknoten gefunden wird.
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// Wird aufgerufen, wenn im Dokument ein Image-Knoten gefunden wird.
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// Wird aufgerufen, wenn im Dokument ein OutlineGroup-Knoten gefunden wird.
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// Wird aufgerufen, wenn im Dokument ein Outline-Knoten gefunden wird.
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// Wird aufgerufen, wenn im Dokument ein OutlineElement-Knoten gefunden wird.
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// Ruft die Gesamtzahl der Knoten des Besuchers ab
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

### Siehe auch

* class [CompositeNode&lt;T&gt;](../compositenode-1)
* class [Page](../page)
* interface [INotebookChildNode](../inotebookchildnode)
* namensraum [Aspose.Note](../../aspose.note)
* Montage [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
