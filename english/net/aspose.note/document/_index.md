---
title: Document
second_title: Aspose.Note for .NET API Reference
description: Represents an Aspose.Note document.
type: docs
weight: 60
url: /net/aspose.note/document/
---
## Document class

Represents an Aspose.Note document.

```csharp
public class Document : CompositeNode<Page>, INotebookChildNode
```

## Constructors

| Name | Description |
| --- | --- |
| [Document](document#constructor)() | Initializes a new instance of the [`Document`](../document) class. Creates a blank OneNote document. |
| [Document](document#constructor_1)(Stream) | Initializes a new instance of the [`Document`](../document) class. Opens an existing OneNote document from a stream. |
| [Document](document#constructor_3)(string) | Initializes a new instance of the [`Document`](../document) class. Opens an existing OneNote document from a file. |
| [Document](document#constructor_2)(Stream, LoadOptions) | Initializes a new instance of the [`Document`](../document) class. Opens an existing OneNote document from a stream. Allows to specify additional options such as an encryption password. |
| [Document](document#constructor_4)(string, LoadOptions) | Initializes a new instance of the [`Document`](../document) class. Opens an existing OneNote document from a file. Allows to specify additional options such as an encryption password. |

## Properties

| Name | Description |
| --- | --- |
| [AutomaticLayoutChangesDetectionEnabled](../../aspose.note/document/automaticlayoutchangesdetectionenabled) { get; set; } | Gets or sets a value indicating whether Aspose.Note performs detection of layout changes automatically. Default value is `true`. |
| [Color](../../aspose.note/document/color) { get; set; } | Gets or sets the color. |
| [CreationTime](../../aspose.note/document/creationtime) { get; set; } | Gets or sets the creation time. |
| [DisplayName](../../aspose.note/document/displayname) { get; set; } | Gets or sets the display name. |
| [Document](../../aspose.note/node/document) { get; } | Gets the document of the node. |
| [FileFormat](../../aspose.note/document/fileformat) { get; } | Gets file format (OneNote 2010, OneNote Online). |
| [FirstChild](../../aspose.note/compositenode`1/firstchild) { get; } |  |
| [Guid](../../aspose.note/document/guid) { get; } | Gets the object's globally unique id. |
| [IsComposite](../../aspose.note/compositenode`1/iscomposite) { get; } |  |
| [LastChild](../../aspose.note/compositenode`1/lastchild) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | Gets the next node at the same node tree level. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | Gets the node type. |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | Gets the parent node. |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | Gets the previous node at the same node tree level. |

## Methods

| Name | Description |
| --- | --- |
| override [Accept](../../aspose.note/document/accept)(DocumentVisitor) | Accepts the visitor of the node. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildfirst)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildlast)(T1) |  |
| [DetectLayoutChanges](../../aspose.note/document/detectlayoutchanges)() | Detects all changes made to the document layout since the previous [`DetectLayoutChanges`](./detectlayoutchanges) call. In case [`AutomaticLayoutChangesDetectionEnabled`](./automaticlayoutchangesdetectionenabled) set to true, used automatically in the beginning of document export. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode`1/getchildnodes)() |  |
| [GetEnumerator](../../aspose.note/compositenode`1/getenumerator)() |  |
| [GetPageHistory](../../aspose.note/document/getpagehistory)(Page) | Gets the [`PageHistory`](../pagehistory) which contains full history for each page presented in a document (the earliest at index 0). The current page revision can be accessed as [`Current`](../pagehistory/current) and contained separately from collection of historical versions. |
| [Import](../../aspose.note/document/import#import)(Stream, PdfImportOptions, MergeOptions) | Imports a set of pages from provided PDF document. |
| [Import](../../aspose.note/document/import#import_1)(string, PdfImportOptions, MergeOptions) | Imports a set of pages from provided PDF document. |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode`1/insertchild)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, IEnumerable&lt;Page&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, params Page[]) |  |
| [Merge](../../aspose.note/document/merge)(IEnumerable&lt;Page&gt;, MergeOptions) | Merges a set of pages to the document. |
| [Print](../../aspose.note/document/print#print)() | Prints the document using the default printer. |
| [Print](../../aspose.note/document/print#print_1)(PrintOptions) | Prints the document using the default printer. |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode`1/removechild)(T1) |  |
| [Save](../../aspose.note/document/save#save)(Stream) | Saves the OneNote document to a stream. |
| [Save](../../aspose.note/document/save#save_3)(string) | Saves the OneNote document to a file. |
| [Save](../../aspose.note/document/save#save_1)(Stream, SaveFormat) | Saves the OneNote document to a stream in the specified format. |
| [Save](../../aspose.note/document/save#save_2)(Stream, SaveOptions) | Saves the OneNote document to a stream using the specified save options. |
| [Save](../../aspose.note/document/save#save_4)(string, SaveFormat) | Saves the OneNote document to a file in the specified format. |
| [Save](../../aspose.note/document/save#save_5)(string, SaveOptions) | Saves the OneNote document to a file using the specified save options. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted)(Stream, out Document) | Checks whether a document from a stream is encrypted. To check it we need to completely load this document. So this method can lead to performance penalty. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_3)(string, out Document) | Checks whether a document from a file is encrypted. To check it we need to completely load this document. So this method can lead to performance penalty. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_1)(Stream, LoadOptions, out Document) | Checks whether a document from a stream is encrypted. To check it we need to completely load this document. So this method can lead to performance penalty. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_2)(Stream, string, out Document) | Checks whether a document from a stream is encrypted. To check it we need to completely load this document. So this method can lead to performance penalty. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_4)(string, LoadOptions, out Document) | Checks whether a document from a file is encrypted. To check it we need to completely load this document. So this method can lead to performance penalty. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_5)(string, string, out Document) | Checks whether a document from a file is encrypted. To check it we need to completely load this document. So this method can lead to performance penalty. |

### Examples

Shows how to sent document to a printer using standard Windows dialog with default options.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
```

Shows how to save a document.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

Shows how to an encrypted document.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

Shows how to save document with encryption.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

Shows how to save a document using SaveFormat enumeration.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

Shows how to save a document using OneSaveOptions.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

Shows how to get page's count of a document.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Pages();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Get number of pages
int count = oneFile.Count();

// Print count on the output screen
Console.WriteLine(count);
```

Shows how to save a document in pdf format using default settings.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Save the document as PDF
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Shows how to save a document in gif format.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// Save the document as gif.
oneFile.Save(dataDir, SaveFormat.Gif);
```

Shows how to set a image quality when saving document as image in JPEG format.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Save the document.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

Shows how to set a image resolution when saving document as image.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Save the document.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

Shows how to get file format of a document.

```csharp
// The path to the documents directory.
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

Shows how to bind a hyperlink to an image.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://image.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

Shows how to save a document to a stream.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// Rewind the stream position back to zero so it is ready for next reader.
dstStream.Seek(0, SeekOrigin.Begin);
```

Shows how to check if a document is password-protected.

```csharp
// The path to the documents directory.
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

Shows how to add new section to a notebook.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Load a OneNote Notebook
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Append a new child to the Notebook
notebook.AppendChild(new Document(dataDir + "Neuer Abschnitt 1.one"));

dataDir = dataDir + "AddChildNode_out.onetoc2";

// Save the Notebook
notebook.Save(dataDir);
```

Shows how to check if a document load is failed because OneNote 2007 format is not supported.

```csharp
// The path to the documents directory.
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

Shows how to restore previous version of a page.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Pages();

// Load OneNote document and get first child           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;           
Page previousPageVersion = document.GetPageHistory(page).Last();

document.RemoveChild(page);
document.AppendChildLast(previousPageVersion);

document.Save(dataDir + "RollBackRevisions_out.one");
```

Shows how to clone a page.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Pages();

// Load OneNote document
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Clone into new document without history
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// Clone into new document with history
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

Shows how to save a document in html format with storing all resources(css/fonts/images) to a separate files.

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

Shows how to save a document to a stream in html format with embedding of all resources(css/fonts/images).

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

Shows how to set text description for an image.

```csharp
// The path to the documents directory.
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

Shows how to get meta information about a page.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Pages();

// Load the document into Aspose.Note.
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

When long OneNote pages are saved in pdf format they are split across pages. The sample shows how to configure the splitting logic of objects located on page's breaks.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// or
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

Shows how to save a document in png format.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initialize ImageSaveOptions object 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // Set page index
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// Save the document as PNG.
oneFile.Save(dataDir, opts);
```

Shows how to edit page's history.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Pages();

// Load OneNote document and get first child           
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

Shows how to check if a document is password-protected by specific password.

```csharp
// The path to the documents directory.
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

Shows how to apply Dark theme style to a Document.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Text();

// Load the document into Aspose.Note.
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

Shows how to pass through content of a notebook.

```csharp
// The path to the documents directory.
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
            // Do something with child document
        }
        else if (notebookChildNode is Notebook)
        {
            // Do something with child notebook
        }
    }
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
```

Shows how to get an image from a document.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Images();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Get all Image nodes
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Save image bytes to a file
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

Shows how to save a document in pdf format.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initialize PdfSaveOptions object
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Set page index of first page to be saved
                              PageIndex = 0,

                              // Set page count
                              PageCount = 1,
                          };

// Save the document as PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Shows how to save a document in pdf format using specific settings.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Initialize PdfSaveOptions object
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Use Jpeg compression
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Quality for JPEG compression
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

Shows how to sent document to a printer using standard Windows dialog with specified options.

```csharp
// The path to the documents directory.
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

Shows how to get content of an attached file.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Attachments();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Sample1.one");

// Get a list of attached file nodes
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// Iterate through all nodes
foreach (AttachedFile file in nodes)
{
    // Load attached file to a stream object
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // Create a local file
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // Copy file stream
            CopyStream(outputStream, fileStream);
        }
    }
}
```

Shows how to get image's meta information.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Images();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Get all Image nodes
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

Shows how to get page's history.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Pages();

// Load OneNote document
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Get first page
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

Shows how to add a file to a document by using filepath.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Attachments();

// Create an object of the Document class
Document doc = new Document();

// Initialize Page class object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialize Outline class object
Outline outline = new Outline(doc);

// Initialize OutlineElement class object
OutlineElement outlineElem = new OutlineElement(doc);

// Initialize AttachedFile class object
AttachedFile attachedFile = new AttachedFile(doc,  dataDir + "attachment.txt");

// Add attached file
outlineElem.AppendChildLast(attachedFile);

// Add outline element node
outline.AppendChildLast(outlineElem);

// Add outline node
page.AppendChildLast(outline);

// Add page node
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileByPath_out.one";
doc.Save(dataDir);
```

Shows how to create a document and save it in html format using default options.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initialize OneNote document
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

// Default style for all text in the document.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// Save into HTML format
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

Shows how to check if a page is a conflict page(i.e. it has changes that OneNote couldn't automatically merge).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// Load OneNote document
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

    // By default conflict pages are just skipped on saving.
    // If mark it as non-conflict then it will be saved as usual one in the history.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

Shows how to add an image from file to a document with user defined properties.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Images();

// Load document from the stream.
Document doc = new Document(dataDir + "Aspose.one");

// Get the first page of the document.
Aspose.Note.Page page = doc.FirstChild;

// Load an image from the file.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Change the image's size according to your needs (optional).
                              Width = 100,
                              Height = 100,

                              // Set the image's location in the page (optional).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // Set image alignment
                              Alignment = HorizontalAlignment.Right
                          };

// Add the image to the page.
page.AppendChildLast(image);
```

Shows how to add a file from a stream to a document.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Attachments();

// Create an object of the Document class
Document doc = new Document();

// Initialize Page class object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialize Outline class object
Outline outline = new Outline(doc);

// Initialize OutlineElement class object
OutlineElement outlineElem = new OutlineElement(doc);

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // Initialize AttachedFile class object and also pass its icon path
    AttachedFile attachedFile = new AttachedFile(doc, dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // Add attached file
    outlineElem.AppendChildLast(attachedFile);
}

// Add outline element node
outline.AppendChildLast(outlineElem);

// Add outline node
page.AppendChildLast(outline);

// Add page node
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileAndSetIcon_out.one";
doc.Save(dataDir);
```

When long OneNote pages are saved in pdf format they are split across pages. The example shows how to configure the splitting logic of objects located on page's breaks.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// Or
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// Or
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// Or
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// Or
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

Shows how to create a document and save in html format specified range of pages.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initialize OneNote document
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Default style for all text in the document.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// Save into HTML format
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

Shows how to create a document with titled page.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Create an object of the Document class
Document doc = new Aspose.Note.Document();

// Initialize Page class object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Default style for all text in the document.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Set page title properties
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Append Page node in the document
doc.AppendChildLast(page);

// Save OneNote document
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

Shows how to add an image from stream to a document.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Images();

// Create an object of the Document class
Document doc = new Document();

// Initialize Page class object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // Load the second image using the image name, extension and stream.
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // Set image alignment
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// Save OneNote document
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

Shows how to add an image from file to a document.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Images();

// Create an object of the Document class
Document doc = new Document();

// Initialize Page class object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialize Outline class object and set offset properties
Outline outline = new Outline(doc);

// Initialize OutlineElement class object
OutlineElement outlineElem = new OutlineElement(doc);

// Load an image by the file path.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Set image alignment
                              Alignment = HorizontalAlignment.Right
                          };

// Add image
outlineElem.AppendChildLast(image);

// Add outline elements
outline.AppendChildLast(outlineElem);

// Add Outline node
page.AppendChildLast(outline);

// Add Page node
doc.AppendChildLast(page);

// Save OneNote document
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

Shows how to create a document with a text.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Create an object of the Document class
Document doc = new Document();

// Initialize Page class object
Page page = new Page(doc);

// Initialize Outline class object
Outline outline = new Outline(doc);

// Initialize OutlineElement class object
OutlineElement outlineElem = new OutlineElement(doc);

// Initialize TextStyle class object and set formatting properties
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Initialize RichText class object and apply text style
RichText text = new RichText(doc) { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// Add RichText node
outlineElem.AppendChildLast(text);

// Add OutlineElement node
outline.AppendChildLast(outlineElem);

// Add Outline node
page.AppendChildLast(outline);

// Add Page node
doc.AppendChildLast(page);

// Save OneNote document
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
doc.Save(dataDir);
```

Shows how to save a document in different formats.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initialize the new Document
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// Initialize the new Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Default style for all text in the document.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Append page node
doc.AppendChildLast(page);

// Save OneNote document in different formats, set text font size and detect layout changes manually.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

Shows how to save a document in html format with storing all resources(css/fonts/images) by using user-defined callbacks.

```csharp
// The code below creates 'documentFolder' folder containing document.html, 'css' folder with 'style.css' file, 'images' folder with images and 'fonts' folder with fonts.
// 'style.css' file will contain at the end the following string "/* This line is appended to stream manually by user */"
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

Shows how to bind a hyperlink to a text.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Tasks();

// Create an object of the Document class
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

// Add outline elements
outline.AppendChildLast(outlineElem);

// Initialize Title class object
Title title = new Title() { TitleText = titleText };

// Initialize Page class object
Page page = new Note.Page() { Title = title };

// Add Outline node
page.AppendChildLast(outline);

// Add Page node
doc.AppendChildLast(page);

// Save OneNote document
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

Shows how to access content of a document using visitor.

```csharp
public static void Run()
{
    // The path to the documents directory.
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // Open the document we want to convert.
    Document doc = new Document(dataDir + "Aspose.one");

    // Create an object that inherits from the DocumentVisitor class.
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // This is the well known Visitor pattern. Get the model to accept a visitor.
    // The model will iterate through itself by calling the corresponding methods
    // on the visitor object (this is called visiting).
    //
    // Note that every node in the object model has the Accept method so the visiting
    // can be executed not only for the whole document, but for any node in the document.
    doc.Accept(myConverter);

    // Once the visiting is complete, we can retrieve the result of the operation,
    // that in this example, has accumulated in the visitor.
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// Simple implementation of saving a document in the plain text format. Implemented as a Visitor.
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
    /// Gets the plain text of the document that was accumulated by the visitor.
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// Adds text to the current output. Honors the enabled/disabled output flag.
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// Called when a RichText node is encountered in the document.
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// Called when a Document node is encountered in the document.
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// Called when a Page node is encountered in the document.
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// Called when processing of a Page node is finished.
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// Called when a Title node is encountered in the document.
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// Called when a Image node is encountered in the document.
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// Called when a OutlineGroup node is encountered in the document.
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// Called when a Outline node is encountered in the document.
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// Called when a OutlineElement node is encountered in the document.
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// Gets the total count of nodes by the Visitor
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

### See Also

* class [CompositeNode&lt;T&gt;](../compositenode-1)
* class [Page](../page)
* interface [INotebookChildNode](../inotebookchildnode)
* namespace [Aspose.Note](../../aspose.note)
* assembly [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
