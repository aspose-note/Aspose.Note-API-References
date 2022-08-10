---
title: DocumentFontsSubsystem
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.Fonts.FontsSubsystemın basit uygulaması. alırFontFamily OS. den nesne
type: docs
weight: 100
url: /tr/net/aspose.note.fonts/documentfontssubsystem/
---
## DocumentFontsSubsystem class

Aspose.Note.Fonts.FontsSubsystem'ın basit uygulaması. alırFontFamily OS. 'den nesne

```csharp
public class DocumentFontsSubsystem : FontsSubsystem
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [DocumentFontsSubsystem](documentfontssubsystem#constructor)(Dictionary&lt;string, string&gt;) | Yeni bir örneğini başlatır[`DocumentFontsSubsystem`](../documentfontssubsystem) sınıf. |
| [DocumentFontsSubsystem](documentfontssubsystem#constructor_1)(Stream, Dictionary&lt;string, string&gt;) | Yeni bir örneğini başlatır[`DocumentFontsSubsystem`](../documentfontssubsystem) sınıf. |
| [DocumentFontsSubsystem](documentfontssubsystem#constructor_2)(string, Dictionary&lt;string, string&gt;) | Yeni bir örneğini başlatır[`DocumentFontsSubsystem`](../documentfontssubsystem) sınıf. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| static [Default](../../aspose.note.fonts/documentfontssubsystem/default) { get; set; } | Statik varsayılan örneği alır veya ayarlar. |
| [DefaultFont](../../aspose.note.fonts/fontssubsystem/defaultfont) { get; } | Varsayılan yazı tipini alır veya ayarlar. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| static [UsingDefaultFont](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfont)(string, Dictionary&lt;string, string&gt;) | Belirtilen varsayılan yazı tipi adını kullanarak yeni DocumentFontsSubsystem örneği oluşturun. |
| static [UsingDefaultFontFromFile](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile)(string, Dictionary&lt;string, string&gt;) | Varsayılan olarak belirtilen dosyadan bir yazı tipi kullanarak yeni DocumentFontsSubsystem örneği oluşturun. |
| static [UsingDefaultFontFromStream](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream)(Stream, Dictionary&lt;string, string&gt;) | Varsayılan olarak belirtilen akıştan bir yazı tipi kullanarak yeni DocumentFontsSubsystem örneği oluşturun. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont)(Stream) | Yazı tipini ekleyin. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont)(string) | Yazı tipini ekleyin. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont)(Stream, string) | Yazı tipini ekleyin. |
| [AddFontSubstitution](../../aspose.note.fonts/fontssubsystem/addfontsubstitution)(string, string) | Yazı tipi değişikliği ekler. |
| virtual [GetFontFamily](../../aspose.note.fonts/fontssubsystem/getfontfamily)(string) | Yazı tipi ailesini alır. |
| [LoadFontsFromFolder](../../aspose.note.fonts/fontssubsystem/loadfontsfromfolder)(string) | Belirtilen klasördeki tüm TrueType yazı tiplerini dahili koleksiyona yükler. |

### Örnekler

Belirtilen varsayılan yazı tipini kullanarak bir belgenin pdf formatında nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Belgeyi PDF olarak kaydet
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

Bir dosyadan varsayılan yazı tipini kullanarak bir belgenin pdf formatında nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Belgeyi PDF olarak kaydet
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

Bir akıştan varsayılan yazı tipini kullanarak bir belgenin pdf formatında nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Belgeyi PDF olarak kaydet
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### Ayrıca bakınız

* class [FontsSubsystem](../fontssubsystem)
* ad alanı [Aspose.Note.Fonts](../../aspose.note.fonts)
* toplantı [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
