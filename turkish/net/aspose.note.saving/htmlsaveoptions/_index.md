---
title: HtmlSaveOptions
second_title: Aspose.Note for .NET API Referansı
description: Belgeyi HTML biçiminde kaydederken ek seçenekleri belirlemeye olanak tanır.
type: docs
weight: 680
url: /tr/net/aspose.note.saving/htmlsaveoptions/
---
## HtmlSaveOptions class

Belgeyi HTML biçiminde kaydederken ek seçenekleri belirlemeye olanak tanır.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions)() | Default_Constructor |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [CssPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/cssperpagegeneration) { get; set; } | StyleSheet dosyasının her yeni sayfa için ayrı ayrı oluşturulup oluşturulmayacağını alır veya ayarlar. |
| [CssSavingCallback](../../aspose.note.saving/htmlsaveoptions/csssavingcallback) { get; set; } | CSS'yi depolamak için kaynak oluşturmak üzere çağrılan geri aramayı alır veya ayarlar. |
| [DocumentPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/documentperpagegeneration) { get; set; } | Sayfa başına belge oluşturmanın etkinleştirilip etkinleştirilmediğini gösteren bir değer alır veya ayarlar. |
| [ExportCss](../../aspose.note.saving/htmlsaveoptions/exportcss) { get; set; } | CSS'nin dışa aktarılma şeklini alır veya ayarlar. |
| [ExportFonts](../../aspose.note.saving/htmlsaveoptions/exportfonts) { get; set; } | Yazı tiplerinin dışa aktarılma şeklini alır veya ayarlar. |
| [ExportImages](../../aspose.note.saving/htmlsaveoptions/exportimages) { get; set; } | Görüntülerin dışa aktarılma şeklini alır veya ayarlar. |
| [FontFaceTypes](../../aspose.note.saving/htmlsaveoptions/fontfacetypes) { get; set; } | Yazı tipi yüz türlerini alır veya ayarlar. |
| [FontSavingCallback](../../aspose.note.saving/htmlsaveoptions/fontsavingcallback) { get; set; } | Yazı tipini depolamak için kaynak oluşturmak üzere çağrılan geri aramayı alır veya ayarlar. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem) { get; set; } | Kaydederken kullanılacak yazı tipi ayarlarını alır veya ayarlar |
| [ImageSavingCallback](../../aspose.note.saving/htmlsaveoptions/imagesavingcallback) { get; set; } | Görüntüyü depolamak için kaynak oluşturmak üzere çağrılan geri aramayı alır veya ayarlar. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount) { get; set; } | Kaydedilecek sayfaların sayısını alır veya ayarlar. Varsayılan olarakMaxValue bu, belgenin tüm sayfalarının oluşturulacağı anlamına gelir. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex) { get; set; } | Kaydedilecek ilk sayfanın dizinini alır veya ayarlar. Varsayılan olarak 0. |
| [PageSavingCallback](../../aspose.note.saving/htmlsaveoptions/pagesavingcallback) { get; set; } | Sayfayı depolamak için kaynak oluşturmak üzere çağrılan geri aramayı alır veya ayarlar. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat) { get; } | Belgenin kaydedildiği biçimi alır. |

### Örnekler

Tüm kaynakları (css/fonts/images) ayrı bir dosyaya depolayarak bir belgenin html formatında nasıl kaydedileceğini gösterir.

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

Tüm kaynakların (css/fonts/images) gömülmesiyle bir belgenin html formatında bir akışa nasıl kaydedileceğini gösterir.

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

Bir belgenin nasıl oluşturulacağını ve belirtilen sayfa aralığının html biçiminde nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// OneNote belgesini başlat
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Belgedeki tüm metinler için varsayılan stil.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// HTML biçiminde kaydet
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

Kullanıcı tanımlı geri aramaları kullanarak tüm kaynakları (css/fonts/images) depolayarak bir belgenin html formatında nasıl kaydedileceğini gösterir.

```csharp
// Aşağıdaki kod, document.html dosyasını içeren 'documentFolder' klasörünü, 'style.css' dosyasını içeren 'css' klasörünü, görüntüleri içeren 'images' klasörünü ve yazı tiplerini içeren 'fonts' klasörünü oluşturur.
// 'style.css' dosyasının sonunda aşağıdaki dizeyi içerecektir "/* Bu satır, kullanıcı tarafından manuel olarak akışa eklenir */"
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

* class [SaveOptions](../saveoptions)
* ad alanı [Aspose.Note.Saving](../../aspose.note.saving)
* toplantı [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
