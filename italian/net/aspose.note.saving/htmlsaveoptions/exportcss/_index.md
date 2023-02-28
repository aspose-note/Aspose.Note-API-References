---
title: HtmlSaveOptions.ExportCss
second_title: Aspose.Note per .NET API Reference
description: HtmlSaveOptions proprietà. Ottiene o imposta il modo in cui il css viene esportato.
type: docs
weight: 50
url: /it/net/aspose.note.saving/htmlsaveoptions/exportcss/
---
## HtmlSaveOptions.ExportCss property

Ottiene o imposta il modo in cui il css viene esportato.

```csharp
public ResourceExportType ExportCss { get; set; }
```

### Esempi

Mostra come salvare un documento in formato html memorizzando tutte le risorse (css/font/immagini) in file separati.

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

Mostra come salvare un documento in uno stream in formato html con l'incorporamento di tutte le risorse (css/font/immagini).

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

### Guarda anche

* enum [ResourceExportType](../../../aspose.note.saving.html/resourceexporttype/)
* class [HtmlSaveOptions](../)
* spazio dei nomi [Aspose.Note.Saving](../../htmlsaveoptions/)
* assemblea [Aspose.Note](../../../)


