---
title: DocumentFontsSubsystem.UsingDefaultFontFromStream
second_title: Aspose.Note for .NET API Referansı
description: DocumentFontsSubsystem yöntem. Varsayılan olarak belirtilen akıştan bir yazı tipi kullanarak yeni DocumentFontsSubsystem örneği oluşturun.
type: docs
weight: 50
url: /tr/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream/
---
## DocumentFontsSubsystem.UsingDefaultFontFromStream method

Varsayılan olarak belirtilen akıştan bir yazı tipi kullanarak yeni DocumentFontsSubsystem örneği oluşturun.

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromStream(Stream defaultFontStream, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| defaultFontStream | Stream | Varsayılan yazı tipi adını içeren akış. |
| fontsSubstitutions | Dictionary`2 | Yazı tipi değişiklikleri. |

### Geri dönüş değeri

[`DocumentFontsSubsystem`](../) .

### Örnekler

Bir akıştan varsayılan yazı tipi kullanılarak bir belgenin pdf biçiminde nasıl kaydedileceğini gösterir.

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

* class [DocumentFontsSubsystem](../)
* ad alanı [Aspose.Note.Fonts](../../documentfontssubsystem/)
* toplantı [Aspose.Note](../../../)


