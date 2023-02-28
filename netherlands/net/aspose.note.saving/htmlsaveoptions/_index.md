---
title: Class HtmlSaveOptions
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.Saving.HtmlSaveOptions klas. Maakt het mogelijk om extra opties op te geven bij het opslaan van documenten in HTMLindeling.
type: docs
weight: 700
url: /nl/net/aspose.note.saving/htmlsaveoptions/
---
## HtmlSaveOptions class

Maakt het mogelijk om extra opties op te geven bij het opslaan van documenten in HTML-indeling.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions/)() | De standaard constructeur. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [CssPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/cssperpagegeneration/) { get; set; } | Hiermee wordt bepaald of het StyleSheet-bestand voor elke nieuwe pagina afzonderlijk wordt gegenereerd. |
| [CssSavingCallback](../../aspose.note.saving/htmlsaveoptions/csssavingcallback/) { get; set; } | Haalt of stelt de callback in die wordt aangeroepen om bronnen te maken om CSS op te slaan. |
| [DocumentPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/documentperpagegeneration/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of het genereren van documenten per pagina is ingeschakeld. |
| [ExportCss](../../aspose.note.saving/htmlsaveoptions/exportcss/) { get; set; } | Hiermee wordt de manier waarop css wordt geëxporteerd opgehaald of ingesteld. |
| [ExportFonts](../../aspose.note.saving/htmlsaveoptions/exportfonts/) { get; set; } | Hiermee wordt de manier waarop lettertypen worden geëxporteerd opgehaald of ingesteld. |
| [ExportImages](../../aspose.note.saving/htmlsaveoptions/exportimages/) { get; set; } | Ophalen of instellen van de manier waarop afbeeldingen worden geëxporteerd. |
| [FontFaceTypes](../../aspose.note.saving/htmlsaveoptions/fontfacetypes/) { get; set; } | Haalt of stelt de lettertypen in. |
| [FontSavingCallback](../../aspose.note.saving/htmlsaveoptions/fontsavingcallback/) { get; set; } | Haalt of stelt de callback in die wordt aangeroepen om een bron te maken om het lettertype op te slaan. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | Haalt lettertype-instellingen op of stelt deze in om te gebruiken tijdens het opslaan |
| [ImageSavingCallback](../../aspose.note.saving/htmlsaveoptions/imagesavingcallback/) { get; set; } | Haalt of stelt de callback in die wordt aangeroepen om een bron te maken om de afbeelding op te slaan. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | Haalt het aantal op te slaan pagina's op of stelt het in. Standaard isMaxValue wat betekent dat alle pagina's van het document worden weergegeven. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | Haalt of stelt de index in van de eerste pagina die moet worden opgeslagen. Standaard is 0. |
| [PageSavingCallback](../../aspose.note.saving/htmlsaveoptions/pagesavingcallback/) { get; set; } | Haalt of stelt de callback in die wordt aangeroepen om een resource te maken om de pagina op te slaan. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | Haalt de indeling op waarin het document is opgeslagen. |

### Voorbeelden

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

### Zie ook

* class [SaveOptions](../saveoptions/)
* naamruimte [Aspose.Note.Saving](../../aspose.note.saving/)
* montage [Aspose.Note](../../)


