---
title: HtmlSaveOptions.ExportImages
second_title: Aspose.Note for .NET API Referansı
description: HtmlSaveOptions mülk. Resimlerin dışa aktarılma şeklini alır veya ayarlar.
type: docs
weight: 70
url: /tr/net/aspose.note.saving/htmlsaveoptions/exportimages/
---
## HtmlSaveOptions.ExportImages property

Resimlerin dışa aktarılma şeklini alır veya ayarlar.

```csharp
public ResourceExportType ExportImages { get; set; }
```

### Örnekler

Tüm kaynakları (css/fonts/images) ayrı bir dosyaya kaydederek bir belgenin html formatında nasıl kaydedileceğini gösterir.

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

Tüm kaynakların (css/fonts/images) gömülmesiyle bir belgenin html biçiminde bir akışa nasıl kaydedileceğini gösterir.

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

### Ayrıca bakınız

* enum [ResourceExportType](../../../aspose.note.saving.html/resourceexporttype/)
* class [HtmlSaveOptions](../)
* ad alanı [Aspose.Note.Saving](../../htmlsaveoptions/)
* toplantı [Aspose.Note](../../../)


