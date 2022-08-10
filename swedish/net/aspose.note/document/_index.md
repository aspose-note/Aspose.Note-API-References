---
title: Document
second_title: Aspose.Note för .NET API-referens
description: Representerar ett Aspose.Note-dokument.
type: docs
weight: 60
url: /sv/net/aspose.note/document/
---
## Document class

Representerar ett Aspose.Note-dokument.

```csharp
public class Document : CompositeNode<Page>, INotebookChildNode
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [Document](document#constructor)() | Initierar en ny instans av[`Document`](../document) class. Skapar ett tomt OneNote-dokument. |
| [Document](document#constructor_1)(Stream) | Initierar en ny instans av[`Document`](../document) class. Öppnar ett befintligt OneNote-dokument från en ström. |
| [Document](document#constructor_3)(string) | Initierar en ny instans av[`Document`](../document) class. Öppnar ett befintligt OneNote-dokument från en fil. |
| [Document](document#constructor_2)(Stream, LoadOptions) | Initierar en ny instans av[`Document`](../document) class. Öppnar ett befintligt OneNote-dokument från en ström. Tillåter att ange ytterligare alternativ såsom ett krypteringslösenord. |
| [Document](document#constructor_4)(string, LoadOptions) | Initierar en ny instans av[`Document`](../document) class. Öppnar ett befintligt OneNote-dokument från en fil. Tillåter att ange ytterligare alternativ såsom ett krypteringslösenord. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [AutomaticLayoutChangesDetectionEnabled](../../aspose.note/document/automaticlayoutchangesdetectionenabled) { get; set; } | Hämtar eller ställer in ett värde som anger om Aspose.Note utför detektering av layoutändringar automatiskt. Standardvärdet är`Sann` . |
| [Color](../../aspose.note/document/color) { get; set; } | Hämtar eller ställer in färgen. |
| [CreationTime](../../aspose.note/document/creationtime) { get; set; } | Hämtar eller ställer in skapelsetiden. |
| [DisplayName](../../aspose.note/document/displayname) { get; set; } | Hämtar eller ställer in visningsnamnet. |
| [Document](../../aspose.note/node/document) { get; } | Hämtar dokumentet för noden. |
| [FileFormat](../../aspose.note/document/fileformat) { get; } | Hämtar filformat (OneNote 2010, OneNote Online). |
| [FirstChild](../../aspose.note/compositenode`1/firstchild) { get; } |  |
| [Guid](../../aspose.note/document/guid) { get; } | Får objektets globalt unika id. |
| [IsComposite](../../aspose.note/compositenode`1/iscomposite) { get; } |  |
| [LastChild](../../aspose.note/compositenode`1/lastchild) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | Hämtar nästa nod på samma nodträdsnivå. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | Hämtar nodtypen. |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | Hämtar den överordnade noden. |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | Hämtar föregående nod på samma nodträdsnivå. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| override [Accept](../../aspose.note/document/accept)(DocumentVisitor) | Accepterar besökaren av noden. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildfirst)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildlast)(T1) |  |
| [DetectLayoutChanges](../../aspose.note/document/detectlayoutchanges)() | Upptäcker alla ändringar som gjorts i dokumentlayouten sedan föregående[`DetectLayoutChanges`](./detectlayoutchanges) ring. I fall[`AutomaticLayoutChangesDetectionEnabled`](./automaticlayoutchangesdetectionenabled) inställd på sant, används automatiskt i början av dokumentexporten. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode`1/getchildnodes)() |  |
| [GetEnumerator](../../aspose.note/compositenode`1/getenumerator)() |  |
| [GetPageHistory](../../aspose.note/document/getpagehistory)(Page) | Får[`PageHistory`](../pagehistory) som innehåller fullständig historik för varje sida som presenteras i ett dokument (tidigast vid index 0). Den aktuella sidversionen kan nås som[`Current`](../pagehistory/current)och finns separat från samlingen av historiska versioner. |
| [Import](../../aspose.note/document/import#import)(Stream, PdfImportOptions, MergeOptions) | Importerar en uppsättning sidor från medföljande PDF-dokument. |
| [Import](../../aspose.note/document/import#import_1)(string, PdfImportOptions, MergeOptions) | Importerar en uppsättning sidor från medföljande PDF-dokument. |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode`1/insertchild)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, IEnumerable&lt;Page&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, params Page[]) |  |
| [Merge](../../aspose.note/document/merge)(IEnumerable&lt;Page&gt;, MergeOptions) | Slår samman en uppsättning sidor till dokumentet. |
| [Print](../../aspose.note/document/print#print)() | Skriver ut dokumentet med standardskrivaren. |
| [Print](../../aspose.note/document/print#print_1)(PrintOptions) | Skriver ut dokumentet med standardskrivaren. |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode`1/removechild)(T1) |  |
| [Save](../../aspose.note/document/save#save)(Stream) | Sparar OneNote-dokumentet i en ström. |
| [Save](../../aspose.note/document/save#save_3)(string) | Sparar OneNote-dokumentet till en fil. |
| [Save](../../aspose.note/document/save#save_1)(Stream, SaveFormat) | Sparar OneNote-dokumentet i en ström i det angivna formatet. |
| [Save](../../aspose.note/document/save#save_2)(Stream, SaveOptions) | Sparar OneNote-dokumentet i en ström med de angivna sparalternativen. |
| [Save](../../aspose.note/document/save#save_4)(string, SaveFormat) | Sparar OneNote-dokumentet till en fil i det angivna formatet. |
| [Save](../../aspose.note/document/save#save_5)(string, SaveOptions) | Sparar OneNote-dokumentet till en fil med de angivna sparalternativen. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted)(Stream, out Document) | Kontrollerar om ett dokument från en ström är krypterat. För att kontrollera det måste vi ladda det här dokumentet helt. Så den här metoden kan leda till prestationsstraff. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_3)(string, out Document) | Kontrollerar om ett dokument från en fil är krypterat. För att kontrollera det måste vi ladda det här dokumentet helt. Så den här metoden kan leda till prestationsstraff. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_1)(Stream, LoadOptions, out Document) | Kontrollerar om ett dokument från en ström är krypterat. För att kontrollera det måste vi ladda det här dokumentet helt. Så den här metoden kan leda till prestationsstraff. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_2)(Stream, string, out Document) | Kontrollerar om ett dokument från en ström är krypterat. För att kontrollera det måste vi ladda det här dokumentet helt. Så den här metoden kan leda till prestationsstraff. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_4)(string, LoadOptions, out Document) | Kontrollerar om ett dokument från en fil är krypterat. För att kontrollera det måste vi ladda det här dokumentet helt. Så den här metoden kan leda till prestationsstraff. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_5)(string, string, out Document) | Kontrollerar om ett dokument från en fil är krypterat. För att kontrollera det måste vi ladda det här dokumentet helt. Så den här metoden kan leda till prestationsstraff. |

### Exempel

Visar hur man skickar dokument till en skrivare med standard Windows-dialogruta med standardalternativ.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
```

Visar hur man sparar ett dokument.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

Visar hur man gör ett krypterat dokument.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

Visar hur man sparar dokument med kryptering.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

Visar hur man sparar ett dokument med hjälp av SaveFormat-uppräkning.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

Visar hur man sparar ett dokument med OneSaveOptions.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

Visar hur man får sidantal för ett dokument.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Pages();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Få antal sidor
int count = oneFile.Count();

// Utskriftsräkning på utdataskärmen
Console.WriteLine(count);
```

Visar hur man sparar ett dokument i pdf-format med standardinställningar.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Spara dokumentet som PDF
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Visar hur man sparar ett dokument i gif-format.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// Spara dokumentet som gif.
oneFile.Save(dataDir, SaveFormat.Gif);
```

Visar hur du ställer in en bildkvalitet när du sparar dokument som bild i JPEG-format.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Spara dokumentet.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

Visar hur du ställer in en bildupplösning när du sparar dokument som bild.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Spara dokumentet.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

Visar hur man får filformat för ett dokument.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");
switch (document.FileFormat)
{
    case FileFormat.OneNote2010:
        // Process OneNote 2010
        break;
    case FileFormat.OneNoteOnline:
        // Process OneNote Online
        break;
}
```

Visar hur man binder en hyperlänk till en bild.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://image.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

Visar hur man sparar ett dokument i en ström.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// Spola tillbaka streampositionen till noll så att den är redo för nästa läsare.
dstStream.Seek(0, SeekOrigin.Begin);
```

Visar hur man kontrollerar om ett dokument är lösenordsskyddat.

```csharp
// Sökvägen till dokumentkatalogen.
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

Visar hur du kontrollerar om en dokumentladdning misslyckades eftersom OneNote 2007-formatet inte stöds.

```csharp
// Sökvägen till dokumentkatalogen.
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

Visar hur man återställer tidigare version av en sida.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Pages();

// Ladda OneNote-dokument och skaffa första barn           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;           
Page previousPageVersion = document.GetPageHistory(page).Last();

document.RemoveChild(page);
document.AppendChildLast(previousPageVersion);

document.Save(dataDir + "RollBackRevisions_out.one");
```

Visar hur man klona en sida.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Pages();

// Ladda OneNote-dokument
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Klona till nytt dokument utan historik
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// Klona in i ett nytt dokument med historik
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

Visar hur man sparar ett dokument i html-format med att lagra alla resurser (css/fonts/images) till en separat fil.

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

Visar hur man sparar ett dokument till en stream i html-format med inbäddning av alla resurser (css/fonts/images).

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

Visar hur man ställer in textbeskrivning för en bild.

```csharp
// Sökvägen till dokumentkatalogen.
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

Visar hur man får metainformation om en sida.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Pages();

// Ladda dokumentet i Aspose.Note.
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

När långa OneNote-sidor sparas i pdf-format delas de upp på sidor. Exemplet visar hur man konfigurerar uppdelningslogiken för objekt som finns på sidavbrott.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// eller
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

Visar hur man sparar ett dokument i png-format.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initiera ImageSaveOptions-objekt 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // Ställ in sidindex
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// Spara dokumentet som PNG.
oneFile.Save(dataDir, opts);
```

Visar hur man redigerar sidans historik.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Pages();

// Ladda OneNote-dokument och skaffa första barn           
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

Visar hur man kontrollerar om ett dokument är lösenordsskyddat med ett specifikt lösenord.

```csharp
// Sökvägen till dokumentkatalogen.
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

Visar hur man hämtar en bild från ett dokument.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Images();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Hämta alla bildnoder
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Spara bildbytes till en fil
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

Visar hur man sparar ett dokument i pdf-format.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initiera PdfSaveOptions-objekt
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Ställ in sidindex för första sidan som ska sparas
                              PageIndex = 0,

                              // Ställ in sidantal
                              PageCount = 1,
                          };

// Spara dokumentet som PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Visar hur man sparar ett dokument i pdf-format med specifika inställningar.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Initiera PdfSaveOptions-objekt
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Använd Jpeg-komprimering
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Kvalitet för JPEG-komprimering
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

Visar hur man skickar dokument till en skrivare med standard Windows-dialogruta med angivna alternativ.

```csharp
// Sökvägen till dokumentkatalogen.
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

Visar hur man får bildens metainformation.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Images();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Hämta alla bildnoder
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

Visar hur man får innehållet i en bifogad fil.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Attachments();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Sample1.one");

// Få en lista över bifogade filnoder
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// Iterera genom alla noder
foreach (AttachedFile file in nodes)
{
    // Ladda bifogad fil till ett strömobjekt
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // Skapa en lokal fil
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // Kopiera filström
            CopyStream(outputStream, fileStream);
        }
    }
}
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

Visar hur man lägger till en fil i ett dokument med hjälp av filsökväg.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Attachments();

// Skapa ett objekt av klassen Document
Document doc = new Document();

// Initiera Sidklassobjekt
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initiera Outline-klassobjekt
Outline outline = new Outline(doc);

// Initiera OutlineElement-klassobjekt
OutlineElement outlineElem = new OutlineElement(doc);

// Initiera AttachedFile-klassobjektet
AttachedFile attachedFile = new AttachedFile(doc,  dataDir + "attachment.txt");

// Lägg till bifogad fil
outlineElem.AppendChildLast(attachedFile);

// Lägg till nod för dispositionselement
outline.AppendChildLast(outlineElem);

// Lägg till dispositionsnod
page.AppendChildLast(outline);

// Lägg till sidnod
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileByPath_out.one";
doc.Save(dataDir);
```

Visar hur man skapar ett dokument och sparar det i html-format med standardalternativ.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initiera OneNote-dokument
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

// Standardstil för all text i dokumentet.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// Spara i HTML-format
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

Visar hur man kontrollerar om en sida är en konfliktsida (dvs. den har ändringar som OneNote inte kunde slå samman automatiskt).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// Ladda OneNote-dokument
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

    // Som standard hoppas konfliktsidor bara över när du sparar.
    // Om det markeras som icke-konflikt kommer det att sparas som vanligt i historiken.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

Visar hur man lägger till en bild från fil till ett dokument med användardefinierade egenskaper.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Images();

// Ladda dokument från strömmen.
Document doc = new Document(dataDir + "Aspose.one");

// Hämta den första sidan av dokumentet.
Aspose.Note.Page page = doc.FirstChild;

// Ladda en bild från filen.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Ändra bildens storlek efter dina behov (valfritt).
                              Width = 100,
                              Height = 100,

                              // Ställ in bildens plats på sidan (valfritt).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // Ställ in bildjustering
                              Alignment = HorizontalAlignment.Right
                          };

// Lägg till bilden på sidan.
page.AppendChildLast(image);
```

Visar hur man lägger till en fil från en ström till ett dokument.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Attachments();

// Skapa ett objekt av klassen Document
Document doc = new Document();

// Initiera Sidklassobjekt
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initiera Outline-klassobjekt
Outline outline = new Outline(doc);

// Initiera OutlineElement-klassobjekt
OutlineElement outlineElem = new OutlineElement(doc);

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // Initiera AttachedFile-klassobjektet och skicka även dess ikonsökväg
    AttachedFile attachedFile = new AttachedFile(doc, dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // Lägg till bifogad fil
    outlineElem.AppendChildLast(attachedFile);
}

// Lägg till nod för dispositionselement
outline.AppendChildLast(outlineElem);

// Lägg till dispositionsnod
page.AppendChildLast(outline);

// Lägg till sidnod
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileAndSetIcon_out.one";
doc.Save(dataDir);
```

När långa OneNote-sidor sparas i pdf-format delas de upp på sidor. Exemplet visar hur man konfigurerar uppdelningslogiken för objekt som finns på sidavbrott.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// Eller
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// Eller
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// Eller
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// Eller
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

Visar hur man skapar ett dokument och sparar i html-format specificerat antal sidor.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initiera OneNote-dokument
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Standardstil för all text i dokumentet.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// Spara i HTML-format
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

Visar hur man skapar ett dokument med titelsida.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Skapa ett objekt av klassen Document
Document doc = new Aspose.Note.Document();

// Initiera Sidklassobjekt
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Standardstil för all text i dokumentet.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Ställ in sidtitelegenskaper
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Lägg till sidnod i dokumentet
doc.AppendChildLast(page);

// Spara OneNote-dokument
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

Visar hur man lägger till en bild från ström till ett dokument.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Images();

// Skapa ett objekt av klassen Document
Document doc = new Document();

// Initiera Sidklassobjekt
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // Ladda den andra bilden med bildnamnet, tillägget och strömmen.
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // Ställ in bildjustering
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// Spara OneNote-dokument
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

Visar hur man lägger till en bild från fil till ett dokument.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Images();

// Skapa ett objekt av klassen Document
Document doc = new Document();

// Initiera Sidklassobjekt
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initiera Outline-klassobjektet och ställ in offsetegenskaper
Outline outline = new Outline(doc);

// Initiera OutlineElement-klassobjekt
OutlineElement outlineElem = new OutlineElement(doc);

// Ladda en bild efter filsökvägen.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Ställ in bildjustering
                              Alignment = HorizontalAlignment.Right
                          };

// Lägg till bild
outlineElem.AppendChildLast(image);

// Lägg till konturelement
outline.AppendChildLast(outlineElem);

// Lägg till Outline-nod
page.AppendChildLast(outline);

// Lägg till sidnod
doc.AppendChildLast(page);

// Spara OneNote-dokument
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

Visar hur man skapar ett dokument med en text.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Skapa ett objekt av klassen Document
Document doc = new Document();

// Initiera Sidklassobjekt
Page page = new Page(doc);

// Initiera Outline-klassobjekt
Outline outline = new Outline(doc);

// Initiera OutlineElement-klassobjekt
OutlineElement outlineElem = new OutlineElement(doc);

// Initiera TextStyle-klassobjektet och ställ in formateringsegenskaper
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Initiera RichText-klassobjekt och tillämpa textstil
RichText text = new RichText(doc) { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// Lägg till RichText-nod
outlineElem.AppendChildLast(text);

// Lägg till OutlineElement-nod
outline.AppendChildLast(outlineElem);

// Lägg till Outline-nod
page.AppendChildLast(outline);

// Lägg till sidnod
doc.AppendChildLast(page);

// Spara OneNote-dokument
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
doc.Save(dataDir);
```

Visar hur man sparar ett dokument i olika format.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initiera det nya dokumentet
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// Initiera den nya sidan
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Standardstil för all text i dokumentet.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Lägg till sidnod
doc.AppendChildLast(page);

// Spara OneNote-dokument i olika format, ställ in textstorlek och upptäck layoutändringar manuellt.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

Visar hur man sparar ett dokument i html-format med lagring av alla resurser (css/fonts/images) genom att använda användardefinierade callbacks.

```csharp
// Koden nedan skapar 'documentFolder'-mappen som innehåller document.html, 'css'-mappen med 'style.css'-filen, 'images'-mappen med bilder och 'fonts'-mappen med typsnitt.
// 'style.css'-filen kommer att innehålla i slutet följande sträng "/* Denna rad har lagts till för att streama manuellt av användaren */"
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

Visar hur man binder en hyperlänk till en text.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Tasks();

// Skapa ett objekt av klassen Document
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

// Lägg till konturelement
outline.AppendChildLast(outlineElem);

// Initiera Title-klassobjekt
Title title = new Title() { TitleText = titleText };

// Initiera Sidklassobjekt
Page page = new Note.Page() { Title = title };

// Lägg till Outline-nod
page.AppendChildLast(outline);

// Lägg till sidnod
doc.AppendChildLast(page);

// Spara OneNote-dokument
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

Visar hur man kommer åt innehållet i ett dokument med hjälp av besökare.

```csharp
public static void Run()
{
    // Sökvägen till dokumentkatalogen.
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // Öppna dokumentet vi vill konvertera.
    Document doc = new Document(dataDir + "Aspose.one");

    // Skapa ett objekt som ärver från klassen DocumentVisitor.
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // Detta är det välkända besökarmönstret. Få modellen att ta emot en besökare.
    // Modellen kommer att iterera genom sig själv genom att anropa motsvarande metoder
    // på besöksobjektet (detta kallas att besöka).
    //
    // Observera att varje nod i objektmodellen har Accept-metoden så att den besöker
    // kan köras inte bara för hela dokumentet, utan för vilken nod som helst i dokumentet.
    doc.Accept(myConverter);

    // När besöket är klart kan vi hämta resultatet av operationen,
    // som i det här exemplet har ackumulerats i besökaren.
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// Enkel implementering av att spara ett dokument i vanlig textformat. Implementerad som besökare.
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
    /// Hämtar vanlig text av dokumentet som samlades av besökaren.
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// Lägger till text till den aktuella utgången. Respekterar den aktiverade/avaktiverade utgångsflaggan.
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// Anropas när en RichText-nod påträffas i dokumentet.
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// Anropas när en dokumentnod påträffas i dokumentet.
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// Anropas när en sidnod påträffas i dokumentet.
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// Anropas när bearbetningen av en sidnod är klar.
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// Anropas när en titelnod påträffas i dokumentet.
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// Anropas när en bildnod påträffas i dokumentet.
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// Anropas när en OutlineGroup-nod påträffas i dokumentet.
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// Anropas när en Outline-nod påträffas i dokumentet.
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// Anropas när en OutlineElement-nod påträffas i dokumentet.
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// Får det totala antalet noder av besökaren
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

### Se även

* class [CompositeNode&lt;T&gt;](../compositenode-1)
* class [Page](../page)
* interface [INotebookChildNode](../inotebookchildnode)
* namnutrymme [Aspose.Note](../../aspose.note)
* hopsättning [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
