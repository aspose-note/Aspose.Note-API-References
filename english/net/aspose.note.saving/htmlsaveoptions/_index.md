---
title: HtmlSaveOptions
second_title: Aspose.Note for .NET API Reference
description: 
type: docs
weight: 640
url: /net/aspose.note.saving/htmlsaveoptions/
---
## HtmlSaveOptions class

Allows to specify additional options when saving document to HTML format.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [CssPerPageGeneration](cssperpagegeneration) { get; set; } | Gets or sets whether the StyleSheet file will be generated for each new page separately. |
| [CssSavingCallback](csssavingcallback) { get; set; } | Gets or sets the callback that is called to create resource to store CSS. |
| [DocumentPerPageGeneration](documentperpagegeneration) { get; set; } | Gets or sets a value indicating whether document per page generation is enabled. |
| [ExportCss](exportcss) { get; set; } | Gets or sets the way css is exported. |
| [ExportFonts](exportfonts) { get; set; } | Gets or sets the way fonts are exported. |
| [ExportImages](exportimages) { get; set; } | Gets or sets the way images are exported. |
| [FontFaceTypes](fontfacetypes) { get; set; } | Gets or sets the font face types. |
| [FontSavingCallback](fontsavingcallback) { get; set; } | Gets or sets the callback that is called to create resource to store font. |
| [ImageSavingCallback](imagesavingcallback) { get; set; } | Gets or sets the callback that is called to create resource to store image. |
| [PageSavingCallback](pagesavingcallback) { get; set; } | Gets or sets the callback that is called to create resource to store page. |

### Examples

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

### See Also

* class [SaveOptions](../saveoptions)
* namespace [Aspose.Note.Saving](../../aspose.note.saving)
* assembly [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
