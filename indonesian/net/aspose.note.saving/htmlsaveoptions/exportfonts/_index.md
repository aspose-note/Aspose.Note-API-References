---
title: HtmlSaveOptions.ExportFonts
second_title: Aspose.Note untuk Referensi .NET API
description: HtmlSaveOptions Properti. Mendapatkan atau menyetel cara font diekspor.
type: docs
weight: 60
url: /id/net/aspose.note.saving/htmlsaveoptions/exportfonts/
---
## HtmlSaveOptions.ExportFonts property

Mendapatkan atau menyetel cara font diekspor.

```csharp
public ResourceExportType ExportFonts { get; set; }
```

### Contoh

Menunjukkan cara menyimpan dokumen dalam format html dengan menyimpan semua sumber daya (css/font/gambar) ke file terpisah.

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

Menunjukkan cara menyimpan dokumen ke aliran dalam format html dengan menyematkan semua sumber daya (css/font/gambar).

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

### Lihat juga

* enum [ResourceExportType](../../../aspose.note.saving.html/resourceexporttype/)
* class [HtmlSaveOptions](../)
* ruang nama [Aspose.Note.Saving](../../htmlsaveoptions/)
* perakitan [Aspose.Note](../../../)


