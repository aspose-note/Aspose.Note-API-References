---
title: HtmlSaveOptions.FontFaceTypes
second_title: Aspose.Note for .NET API Referansı
description: HtmlSaveOptions mülk. Yazı tipi yüzü türlerini alır veya ayarlar.
type: docs
weight: 80
url: /tr/net/aspose.note.saving/htmlsaveoptions/fontfacetypes/
---
## HtmlSaveOptions.FontFaceTypes property

Yazı tipi yüzü türlerini alır veya ayarlar.

```csharp
public FontFaceType FontFaceTypes { get; set; }
```

### Mülk değeri

Yazı tipi yüzü türleri.

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

Kullanıcı tanımlı geri aramalar kullanarak tüm kaynakları (css/fonts/images) depolayarak bir belgenin html formatında nasıl kaydedileceğini gösterir.

```csharp
// Aşağıdaki kod, document.html'yi içeren 'documentFolder' klasörünü, 'style.css' dosyasını içeren 'css' klasörünü, resimleri içeren 'images' klasörünü ve fontları içeren 'fonts' klasörünü oluşturur.
// 'style.css' dosyası sonunda şu dizeyi içerecektir "/* Bu satır akışa kullanıcı tarafından manuel olarak eklenmiştir */"
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

### Ayrıca bakınız

* enum [FontFaceType](../../../aspose.note.saving.html/fontfacetype/)
* class [HtmlSaveOptions](../)
* ad alanı [Aspose.Note.Saving](../../htmlsaveoptions/)
* toplantı [Aspose.Note](../../../)


