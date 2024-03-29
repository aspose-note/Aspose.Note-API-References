---
title: HtmlSaveOptions.ExportImages
second_title: Aspose.Note for .NET API Reference
description: HtmlSaveOptions property. Gets or sets the way images are exported
type: docs
weight: 70
url: /net/aspose.note.saving/htmlsaveoptions/exportimages/
---
## HtmlSaveOptions.ExportImages property

Gets or sets the way images are exported.

```csharp
public ResourceExportType ExportImages { get; set; }
```

## Examples

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

### See Also

* enum [ResourceExportType](../../../aspose.note.saving.html/resourceexporttype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Note.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Note](../../../)


