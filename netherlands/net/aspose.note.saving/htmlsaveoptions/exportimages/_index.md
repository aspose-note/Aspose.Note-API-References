---
title: HtmlSaveOptions.ExportImages
second_title: Aspose.Note voor .NET API-referentie
description: HtmlSaveOptions eigendom. Ophalen of instellen van de manier waarop afbeeldingen worden geëxporteerd.
type: docs
weight: 70
url: /nl/net/aspose.note.saving/htmlsaveoptions/exportimages/
---
## HtmlSaveOptions.ExportImages property

Ophalen of instellen van de manier waarop afbeeldingen worden geëxporteerd.

```csharp
public ResourceExportType ExportImages { get; set; }
```

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

### Zie ook

* enum [ResourceExportType](../../../aspose.note.saving.html/resourceexporttype/)
* class [HtmlSaveOptions](../)
* naamruimte [Aspose.Note.Saving](../../htmlsaveoptions/)
* montage [Aspose.Note](../../../)


