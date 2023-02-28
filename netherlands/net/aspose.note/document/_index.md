---
title: Class Document
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.Document klas. Vertegenwoordigt een Aspose.Notedocument.
type: docs
weight: 60
url: /nl/net/aspose.note/document/
---
## Document class

Vertegenwoordigt een Aspose.Note-document.

```csharp
public class Document : CompositeNode<Page>, INotebookChildNode
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [Document](document/#constructor)() | Initialiseert een nieuw exemplaar van het`Document` class. Maakt een leeg OneNote-document aan. |
| [Document](document/#constructor_1)(Stream) | Initialiseert een nieuw exemplaar van het`Document` class. Opent een bestaand OneNote-document uit een stream. |
| [Document](document/#constructor_3)(string) | Initialiseert een nieuw exemplaar van het`Document` class. Opent een bestaand OneNote-document vanuit een bestand. |
| [Document](document/#constructor_2)(Stream, LoadOptions) | Initialiseert een nieuw exemplaar van het`Document` class. Opent een bestaand OneNote-document vanuit een stream. Maakt het mogelijk om extra opties op te geven, zoals een coderingswachtwoord. |
| [Document](document/#constructor_4)(string, LoadOptions) | Initialiseert een nieuw exemplaar van het`Document`class. Opent een bestaand OneNote-document vanuit een bestand. Maakt het mogelijk om extra opties op te geven, zoals een coderingswachtwoord. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [AutomaticLayoutChangesDetectionEnabled](../../aspose.note/document/automaticlayoutchangesdetectionenabled/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of Aspose.Note automatische detectie van lay-outwijzigingen uitvoert. Standaardwaarde is`WAAR` . |
| [Color](../../aspose.note/document/color/) { get; set; } | Krijgt of stelt de kleur in. |
| [CreationTime](../../aspose.note/document/creationtime/) { get; set; } | Haalt of stelt de aanmaaktijd in. |
| [DisplayName](../../aspose.note/document/displayname/) { get; set; } | Haalt de weergavenaam op of stelt deze in. |
| [Document](../../aspose.note/node/document/) { get; } | Haalt het document van het knooppunt op. |
| [FileFormat](../../aspose.note/document/fileformat/) { get; } | Krijgt bestandsindeling (OneNote 2010, OneNote Online). |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [Guid](../../aspose.note/document/guid/) { get; } | Haalt de wereldwijd unieke id van het object op. |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Haalt het volgende knooppunt op op hetzelfde knooppuntboomniveau. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Haalt het knooppunttype op. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Haalt het bovenliggende knooppunt op. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Haalt het vorige knooppunt op hetzelfde knooppuntboomniveau. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| override [Accept](../../aspose.note/document/accept/)(DocumentVisitor) | Accepteert de bezoeker van de node. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| [DetectLayoutChanges](../../aspose.note/document/detectlayoutchanges/)() | Detecteert alle wijzigingen die sinds de vorige in de documentlay-out zijn aangebracht[`DetectLayoutChanges`](./detectlayoutchanges/) bel. Voor het geval dat[`AutomaticLayoutChangesDetectionEnabled`](./automaticlayoutchangesdetectionenabled/) ingesteld op waar, automatisch gebruikt bij het begin van documentexport. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| [GetPageHistory](../../aspose.note/document/getpagehistory/)(Page) | Krijgt de[`PageHistory`](../pagehistory/) die de volledige geschiedenis bevat voor elke pagina die in een document wordt gepresenteerd (de vroegste op index 0). De huidige paginarevisie is toegankelijk als[`Current`](../pagehistory/current/) en afzonderlijk opgenomen in de verzameling historische versies. |
| [Import](../../aspose.note/document/import/#import)(Stream, PdfImportOptions, MergeOptions) | Importeert een set pagina's uit het meegeleverde PDF-document. |
| [Import](../../aspose.note/document/import/#import_1)(string, PdfImportOptions, MergeOptions) | Importeert een set pagina's uit het meegeleverde PDF-document. |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;Page&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params Page[]) |  |
| [Merge](../../aspose.note/document/merge/)(IEnumerable&lt;Page&gt;, MergeOptions) | Voegt een reeks pagina's samen in het document. |
| [Print](../../aspose.note/document/print/#print)() | Drukt het document af met de standaardprinter. |
| [Print](../../aspose.note/document/print/#print_1)(PrintOptions) | Drukt het document af met de standaardprinter. |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |
| [Save](../../aspose.note/document/save/#save)(Stream) | Slaat het OneNote-document op in een stream. |
| [Save](../../aspose.note/document/save/#save_3)(string) | Slaat het OneNote-document op in een bestand. |
| [Save](../../aspose.note/document/save/#save_1)(Stream, SaveFormat) | Slaat het OneNote-document op in een stream in de opgegeven indeling. |
| [Save](../../aspose.note/document/save/#save_2)(Stream, SaveOptions) | Slaat het OneNote-document op in een stream met behulp van de opgegeven opslagopties. |
| [Save](../../aspose.note/document/save/#save_4)(string, SaveFormat) | Slaat het OneNote-document op in een bestand in de opgegeven indeling. |
| [Save](../../aspose.note/document/save/#save_5)(string, SaveOptions) | Slaat het OneNote-document op in een bestand met de opgegeven opslagopties. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted)(Stream, out Document) | Controleert of een document uit een stream versleuteld is. Om dit te controleren moeten we dit document volledig laden. Dus deze methode kan leiden tot een prestatiestraf. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_3)(string, out Document) | Controleert of een document uit een bestand versleuteld is. Om dit te controleren moeten we dit document volledig laden. Dus deze methode kan leiden tot een prestatiestraf. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_1)(Stream, LoadOptions, out Document) | Controleert of een document uit een stream versleuteld is. Om dit te controleren moeten we dit document volledig laden. Dus deze methode kan leiden tot een prestatiestraf. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_2)(Stream, string, out Document) | Controleert of een document uit een stream versleuteld is. Om dit te controleren moeten we dit document volledig laden. Dus deze methode kan leiden tot een prestatiestraf. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_4)(string, LoadOptions, out Document) | Controleert of een document uit een bestand versleuteld is. Om dit te controleren moeten we dit document volledig laden. Dus deze methode kan leiden tot een prestatiestraf. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_5)(string, string, out Document) | Controleert of een document uit een bestand versleuteld is. Om dit te controleren moeten we dit document volledig laden. Dus deze methode kan leiden tot een prestatiestraf. |

### Voorbeelden

Laat zien hoe u een document naar een printer kunt sturen met behulp van het standaard Windows-dialoogvenster met standaardopties.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
```

Laat zien hoe u een document opslaat.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

Laat zien hoe u een gecodeerd document maakt.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

Laat zien hoe u een document kunt opslaan met codering.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

Laat zien hoe u een document kunt opslaan met behulp van SaveFormat-opsomming.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

Laat zien hoe u een document kunt opslaan met behulp van OneSaveOptions.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

Laat zien hoe u het aantal pagina's van een document kunt opvragen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Pages();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Haal het aantal pagina's op
int count = oneFile.Count();

// Aantal afdrukken op het uitvoerscherm
Console.WriteLine(count);
```

Laat zien hoe u een document in pdf-indeling kunt opslaan met standaardinstellingen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Sla het document op als PDF
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Laat zien hoe je een document opslaat in gif-formaat.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// Sla het document op als gif.
oneFile.Save(dataDir, SaveFormat.Gif);
```

Laat zien hoe u een afbeeldingskwaliteit instelt wanneer u een document opslaat als afbeelding in JPEG-indeling.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Sla het document op.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

Laat zien hoe u een afbeeldingsresolutie instelt bij het opslaan van een document als afbeelding.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Sla het document op.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

Laat zien hoe u de bestandsindeling van een document kunt krijgen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");
switch (document.FileFormat)
{
    case FileFormat.OneNote2010:
        // Verwerk OneNote 2010
        break;
    case FileFormat.OneNoteOnline:
        // Verwerk OneNote online
        break;
}
```

Laat zien hoe u een hyperlink aan een afbeelding koppelt.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://afbeelding.com"};

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

Laat zien hoe u een document opslaat in een stream.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// Spoel de streampositie terug naar nul zodat deze klaar is voor de volgende lezer.
dstStream.Seek(0, SeekOrigin.Begin);
```

Laat zien hoe u kunt controleren of een document met een wachtwoord is beveiligd.

```csharp
// Het pad naar de documentenmap.
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

Laat zien hoe u kunt controleren of het laden van een document is mislukt omdat de OneNote 2007-indeling niet wordt ondersteund.

```csharp
// Het pad naar de documentenmap.
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

Laat zien hoe u de vorige versie van een pagina kunt herstellen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Pages();

// Laad een OneNote-document en krijg het eerste kind           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;           
Page previousPageVersion = document.GetPageHistory(page).Last();

document.RemoveChild(page);
document.AppendChildLast(previousPageVersion);

document.Save(dataDir + "RollBackRevisions_out.one");
```

Laat zien hoe u een pagina kunt klonen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Pages();

// Laad OneNote-document
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Kloon in een nieuw document zonder geschiedenis
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// Kloon in een nieuw document met geschiedenis
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

Laat zien hoe u een document in html-indeling opslaat met alle bronnen (css/fonts/afbeeldingen) in afzonderlijke bestanden.

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

Laat zien hoe u een document opslaat in een stream in html-indeling met inbedding van alle bronnen (css/fonts/afbeeldingen).

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

Laat zien hoe u een tekstbeschrijving voor een afbeelding instelt.

```csharp
// Het pad naar de documentenmap.
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

Laat zien hoe u meta-informatie over een pagina kunt krijgen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Pages();

// Laad het document in Aspose.Note.
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

Wanneer lange OneNote-pagina's in pdf-indeling worden opgeslagen, worden ze over pagina's verdeeld. Het voorbeeld laat zien hoe u de splitsingslogica configureert van objecten die zich op pagina-einden bevinden.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// of
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

Laat zien hoe u een document opslaat in png-indeling.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initialiseer het ImageSaveOptions-object 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // Stel pagina-index in
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// Sla het document op als PNG.
oneFile.Save(dataDir, opts);
```

Laat zien hoe u de geschiedenis van de pagina kunt bewerken.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Pages();

// Laad een OneNote-document en krijg het eerste kind           
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

Laat zien hoe u kunt controleren of een document met een specifiek wachtwoord is beveiligd met een wachtwoord.

```csharp
// Het pad naar de documentenmap.
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

Laat zien hoe u de donkere themastijl toepast op een document.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Text();

// Laad het document in Aspose.Note.
Document doc = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in doc)
{
    page.BackgroundColor = Color.Black;
}

foreach (var node in doc.GetChildNodes<RichText>())
{
    var c = node.ParagraphStyle.FontColor;
    if (c.IsEmpty || Math.Abs(c.R - Color.Black.R) + Math.Abs(c.G - Color.Black.G) + Math.Abs(c.B - Color.Black.B) <= 30)
    {
        node.ParagraphStyle.FontColor = Color.White;
    }
}

doc.Save(Path.Combine(dataDir, "AsposeDarkTheme.pdf"));
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

Laat zien hoe u een afbeelding uit een document haalt.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Images();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Haal alle afbeeldingsknooppunten op
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Bewaar afbeeldingsbytes in een bestand
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

Laat zien hoe u een document opslaat in pdf-formaat.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initialiseer het PdfSaveOptions-object
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Stel de pagina-index in van de eerste pagina die moet worden opgeslagen
                              PageIndex = 0,

                              // Stel het aantal pagina's in
                              PageCount = 1,
                          };

// Sla het document op als PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Laat zien hoe u een document in pdf-formaat kunt opslaan met behulp van specifieke instellingen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Initialiseer het PdfSaveOptions-object
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Gebruik JPEG-compressie
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Kwaliteit voor JPEG-compressie
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

Laat zien hoe u een document naar een printer kunt sturen met behulp van het standaard Windows-dialoogvenster met gespecificeerde opties.

```csharp
// Het pad naar de documentenmap.
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

Laat zien hoe u de inhoud van een bijgevoegd bestand kunt ophalen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Attachments();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Sample1.one");

// Krijg een lijst met bijgevoegde bestandsknooppunten
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// Doorloop alle knooppunten
foreach (AttachedFile file in nodes)
{
    // Laad bijgevoegd bestand naar een streamobject
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // Maak een lokaal bestand
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // Bestandsstroom kopiëren
            CopyStream(outputStream, fileStream);
        }
    }
}
```

Laat zien hoe u de meta-informatie van de afbeelding kunt krijgen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Images();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Haal alle afbeeldingsknooppunten op
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

Laat zien hoe een bestand aan een document kan worden toegevoegd met behulp van bestandspad.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Attachments();

// Maak een object van de klasse Document
Document doc = new Document();

// Initialiseer het paginaklasse-object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialiseer het Outline-klassenobject
Outline outline = new Outline(doc);

// Initialiseer het klasseobject OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Initialiseer het klasseobject AttachedFile
AttachedFile attachedFile = new AttachedFile(doc,  dataDir + "attachment.txt");

// Voeg bijgevoegd bestand toe
outlineElem.AppendChildLast(attachedFile);

// Voeg overzichtselementknooppunt toe
outline.AppendChildLast(outlineElem);

// Voeg overzichtsknooppunt toe
page.AppendChildLast(outline);

// Paginaknooppunt toevoegen
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileByPath_out.one";
doc.Save(dataDir);
```

Laat zien hoe u een document maakt en opslaat in html-indeling met standaardopties.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initialiseer OneNote-document
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

// Standaardstijl voor alle tekst in het document.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// Opslaan in HTML-formaat
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

Laat zien hoe u kunt controleren of een pagina een conflictpagina is (dwz dat deze wijzigingen bevat die OneNote niet automatisch kan samenvoegen).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// Laad OneNote-document
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

    // Standaard worden conflictpagina's gewoon overgeslagen bij het opslaan.
    // Als u het als niet-conflict markeert, wordt het zoals gebruikelijk in de geschiedenis opgeslagen.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

Laat zien hoe u een afbeelding uit een bestand toevoegt aan een document met door de gebruiker gedefinieerde eigenschappen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Images();

// Laad document uit de stream.
Document doc = new Document(dataDir + "Aspose.one");

// Haal de eerste pagina van het document op.
Aspose.Note.Page page = doc.FirstChild;

// Laad een afbeelding uit het bestand.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Wijzig de grootte van de afbeelding volgens uw behoeften (optioneel).
                              Width = 100,
                              Height = 100,

                              // Stel de locatie van de afbeelding op de pagina in (optioneel).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // Beelduitlijning instellen
                              Alignment = HorizontalAlignment.Right
                          };

// Voeg de afbeelding toe aan de pagina.
page.AppendChildLast(image);
```

Laat zien hoe u een bestand uit een stroom toevoegt aan een document.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Attachments();

// Maak een object van de klasse Document
Document doc = new Document();

// Initialiseer het paginaklasse-object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialiseer het Outline-klassenobject
Outline outline = new Outline(doc);

// Initialiseer het klasseobject OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // Initialiseer het klasseobject AttachedFile en geef ook het pictogrampad door
    AttachedFile attachedFile = new AttachedFile(doc, dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // Voeg bijgevoegd bestand toe
    outlineElem.AppendChildLast(attachedFile);
}

// Voeg overzichtselementknooppunt toe
outline.AppendChildLast(outlineElem);

// Voeg overzichtsknooppunt toe
page.AppendChildLast(outline);

// Paginaknooppunt toevoegen
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileAndSetIcon_out.one";
doc.Save(dataDir);
```

Wanneer lange OneNote-pagina's in pdf-indeling worden opgeslagen, worden ze over pagina's verdeeld. Het voorbeeld laat zien hoe u de splitsingslogica configureert van objecten die zich op pagina-einden bevinden.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// Of
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// Of
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// Of
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// Of
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

Laat zien hoe u een document maakt en opslaat in een opgegeven paginabereik in html-indeling.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initialiseer OneNote-document
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Standaardstijl voor alle tekst in het document.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// Opslaan in HTML-formaat
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

Laat zien hoe u een document met een titelpagina maakt.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Maak een object van de klasse Document
Document doc = new Aspose.Note.Document();

// Initialiseer het paginaklasse-object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Standaardstijl voor alle tekst in het document.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Stel de eigenschappen van de paginatitel in
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Voeg een paginaknooppunt toe aan het document
doc.AppendChildLast(page);

// Sla OneNote-document op
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

Laat zien hoe u een afbeelding uit een stream toevoegt aan een document.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Images();

// Maak een object van de klasse Document
Document doc = new Document();

// Initialiseer het paginaklasse-object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // Laad de tweede afbeelding met de afbeeldingsnaam, extensie en stream.
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // Beelduitlijning instellen
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// Sla OneNote-document op
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

Laat zien hoe u een afbeelding uit een bestand toevoegt aan een document.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Images();

// Maak een object van de klasse Document
Document doc = new Document();

// Initialiseer het paginaklasse-object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialiseer het Outline-klasseobject en stel offset-eigenschappen in
Outline outline = new Outline(doc);

// Initialiseer het klasseobject OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Laad een afbeelding via het bestandspad.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Beelduitlijning instellen
                              Alignment = HorizontalAlignment.Right
                          };

// Voeg afbeelding toe
outlineElem.AppendChildLast(image);

// Voeg overzichtselementen toe
outline.AppendChildLast(outlineElem);

// Overzichtsknooppunt toevoegen
page.AppendChildLast(outline);

// Paginaknooppunt toevoegen
doc.AppendChildLast(page);

// Sla OneNote-document op
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

Laat zien hoe je een document maakt met een tekst.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Maak een object van de klasse Document
Document doc = new Document();

// Initialiseer het paginaklasse-object
Page page = new Page(doc);

// Initialiseer het Outline-klassenobject
Outline outline = new Outline(doc);

// Initialiseer het klasseobject OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Initialiseer het klasseobject TextStyle en stel opmaakeigenschappen in
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Initialiseer het RichText-klasseobject en pas tekststijl toe
RichText text = new RichText(doc) { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// RichText-knooppunt toevoegen
outlineElem.AppendChildLast(text);

// Voeg een OutlineElement-knooppunt toe
outline.AppendChildLast(outlineElem);

// Overzichtsknooppunt toevoegen
page.AppendChildLast(outline);

// Paginaknooppunt toevoegen
doc.AppendChildLast(page);

// Sla OneNote-document op
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
doc.Save(dataDir);
```

Laat zien hoe u een document in verschillende indelingen kunt opslaan.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initialiseer het nieuwe document
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// Initialiseer de nieuwe pagina
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Standaardstijl voor alle tekst in het document.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Paginaknooppunt toevoegen
doc.AppendChildLast(page);

// Bewaar OneNote-document in verschillende formaten, stel de lettergrootte van tekst in en detecteer lay-outwijzigingen handmatig.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

Laat zien hoe u een document opslaat in html-indeling met opslag van alle bronnen (css/fonts/afbeeldingen) door gebruik te maken van door de gebruiker gedefinieerde callbacks.

```csharp
// De onderstaande code maakt de map 'documentFolder' met daarin document.html, de map 'css' met het bestand 'style.css', de map 'images' met afbeeldingen en de map 'fonts' met lettertypen.
// Het bestand 'style.css' bevat aan het einde de volgende tekenreeks "/* Deze regel is toegevoegd om handmatig door de gebruiker te streamen */"
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

Laat zien hoe u een hyperlink aan een tekst koppelt.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Tasks();

// Maak een object van de klasse Document
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

// Voeg overzichtselementen toe
outline.AppendChildLast(outlineElem);

// Initialiseer het titelklasse-object
Title title = new Title() { TitleText = titleText };

// Initialiseer het paginaklasse-object
Page page = new Note.Page() { Title = title };

// Overzichtsknooppunt toevoegen
page.AppendChildLast(outline);

// Paginaknooppunt toevoegen
doc.AppendChildLast(page);

// Sla OneNote-document op
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

Laat zien hoe u toegang krijgt tot de inhoud van een document met behulp van bezoeker.

```csharp
public static void Run()
{
    // Het pad naar de documentenmap.
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // Open het document dat we willen converteren.
    Document doc = new Document(dataDir + "Aspose.one");

    // Maak een object dat overerft van de klasse DocumentVisitor.
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // Dit is het bekende Visitor-patroon. Laat het model een bezoeker accepteren.
    // Het model herhaalt zichzelf door de overeenkomstige methoden aan te roepen
    // op het bezoekersobject (dit wordt bezoeken genoemd).
    //
    // Merk op dat elk knooppunt in het objectmodel de Accept-methode heeft, dus het bezoeken
    // kan niet alleen voor het hele document worden uitgevoerd, maar voor elk knooppunt in het document.
    doc.Accept(myConverter);

    // Zodra het bezoek is voltooid, kunnen we het resultaat van de operatie ophalen,
    // die zich in dit voorbeeld heeft opgehoopt in de bezoeker.
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// Eenvoudige implementatie van het opslaan van een document in platte tekst. Geïmplementeerd als bezoeker.
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
    /// Krijgt de platte tekst van het document dat door de bezoeker is verzameld.
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// Voegt tekst toe aan de huidige uitvoer. Eert de uitvoervlag ingeschakeld/uitgeschakeld.
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// Aangeroepen wanneer een RichText-knooppunt wordt aangetroffen in het document.
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// Aangeroepen wanneer een documentknooppunt wordt aangetroffen in het document.
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// Aangeroepen wanneer een paginaknooppunt wordt aangetroffen in het document.
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// Opgeroepen wanneer de verwerking van een paginaknooppunt is voltooid.
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// Aangeroepen wanneer een titelknooppunt wordt aangetroffen in het document.
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// Aangeroepen wanneer een afbeeldingsknooppunt wordt aangetroffen in het document.
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// Aangeroepen wanneer een OutlineGroup-knooppunt wordt aangetroffen in het document.
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// Aangeroepen wanneer een Outline-knooppunt wordt aangetroffen in het document.
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// Aangeroepen wanneer een OutlineElement-knooppunt wordt aangetroffen in het document.
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// Krijgt het totale aantal nodes van de bezoeker
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

### Zie ook

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* class [Page](../page/)
* interface [INotebookChildNode](../inotebookchildnode/)
* naamruimte [Aspose.Note](../../aspose.note/)
* montage [Aspose.Note](../../)


