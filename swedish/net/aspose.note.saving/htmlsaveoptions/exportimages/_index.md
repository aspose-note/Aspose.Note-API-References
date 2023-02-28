---
title: HtmlSaveOptions.ExportImages
second_title: Aspose.Note för .NET API-referens
description: HtmlSaveOptions fast egendom. Hämtar eller ställer in hur bilder exporteras.
type: docs
weight: 70
url: /sv/net/aspose.note.saving/htmlsaveoptions/exportimages/
---
## HtmlSaveOptions.ExportImages property

Hämtar eller ställer in hur bilder exporteras.

```csharp
public ResourceExportType ExportImages { get; set; }
```

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

### Se även

* enum [ResourceExportType](../../../aspose.note.saving.html/resourceexporttype/)
* class [HtmlSaveOptions](../)
* namnutrymme [Aspose.Note.Saving](../../htmlsaveoptions/)
* hopsättning [Aspose.Note](../../../)


