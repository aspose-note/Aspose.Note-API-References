---
title: HtmlSaveOptions.ExportCss
second_title: Aspose.Note für .NET-API-Referenz
description: HtmlSaveOptions eigendom. Ruft ab oder legt fest wie CSS exportiert wird.
type: docs
weight: 50
url: /de/net/aspose.note.saving/htmlsaveoptions/exportcss/
---
## HtmlSaveOptions.ExportCss property

Ruft ab oder legt fest, wie CSS exportiert wird.

```csharp
public ResourceExportType ExportCss { get; set; }
```

### Beispiele

Zeigt, wie ein Dokument im HTML-Format gespeichert wird, wobei alle Ressourcen (css/fonts/images) in separaten Dateien gespeichert werden.

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

Zeigt, wie ein Dokument in einem Stream im HTML-Format mit Einbettung aller Ressourcen (css/fonts/images) gespeichert wird.

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

### Siehe auch

* enum [ResourceExportType](../../../aspose.note.saving.html/resourceexporttype/)
* class [HtmlSaveOptions](../)
* namensraum [Aspose.Note.Saving](../../htmlsaveoptions/)
* Montage [Aspose.Note](../../../)


