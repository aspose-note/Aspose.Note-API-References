---
title: HtmlSaveOptions
second_title: Aspose.Note för .NET API-referens
description: Gör det möjligt att ange ytterligare alternativ när du sparar dokument i HTML-format.
type: docs
weight: 680
url: /sv/net/aspose.note.saving/htmlsaveoptions/
---
## HtmlSaveOptions class

Gör det möjligt att ange ytterligare alternativ när du sparar dokument i HTML-format.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions)() | Default_Constructor |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [CssPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/cssperpagegeneration) { get; set; } | Hämtar eller ställer in om StyleSheet-filen ska genereras för varje ny sida separat. |
| [CssSavingCallback](../../aspose.note.saving/htmlsaveoptions/csssavingcallback) { get; set; } | Hämtar eller ställer in återuppringningen som anropas för att skapa resurs för att lagra CSS. |
| [DocumentPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/documentperpagegeneration) { get; set; } | Hämtar eller ställer in ett värde som anger om generering av dokument per sida är aktiverat. |
| [ExportCss](../../aspose.note.saving/htmlsaveoptions/exportcss) { get; set; } | Hämtar eller ställer in hur css exporteras. |
| [ExportFonts](../../aspose.note.saving/htmlsaveoptions/exportfonts) { get; set; } | Hämtar eller ställer in hur teckensnitt exporteras. |
| [ExportImages](../../aspose.note.saving/htmlsaveoptions/exportimages) { get; set; } | Hämtar eller ställer in hur bilder exporteras. |
| [FontFaceTypes](../../aspose.note.saving/htmlsaveoptions/fontfacetypes) { get; set; } | Hämtar eller ställer in teckensnittstyper. |
| [FontSavingCallback](../../aspose.note.saving/htmlsaveoptions/fontsavingcallback) { get; set; } | Hämtar eller ställer in återuppringningen som anropas för att skapa resurs för att lagra teckensnitt. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem) { get; set; } | Hämtar eller ställer in teckensnittets inställningar som ska användas medan de sparas |
| [ImageSavingCallback](../../aspose.note.saving/htmlsaveoptions/imagesavingcallback) { get; set; } | Hämtar eller ställer in återuppringningen som anropas för att skapa resurs för att lagra bild. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount) { get; set; } | Hämtar eller ställer in antalet sidor som ska sparas. Som standard ärMaxValue vilket innebär att alla sidor i dokumentet kommer att renderas. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex) { get; set; } | Hämtar eller ställer in indexet för den första sidan som ska sparas. Som standard är 0. |
| [PageSavingCallback](../../aspose.note.saving/htmlsaveoptions/pagesavingcallback) { get; set; } | Hämtar eller ställer in återuppringningen som anropas för att skapa resurs till butikssida. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat) { get; } | Hämtar formatet som dokumentet sparas i. |

### Exempel

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

### Se även

* class [SaveOptions](../saveoptions)
* namnutrymme [Aspose.Note.Saving](../../aspose.note.saving)
* hopsättning [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
