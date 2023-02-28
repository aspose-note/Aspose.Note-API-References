---
title: DocumentFontsSubsystem.UsingDefaultFontFromFile
second_title: Aspose.Note for .NET API Referansı
description: DocumentFontsSubsystem yöntem. Belirtilen dosyadaki bir yazı tipini varsayılan olarak kullanarak yeni DocumentFontsSubsystem örneği oluşturun.
type: docs
weight: 40
url: /tr/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/
---
## DocumentFontsSubsystem.UsingDefaultFontFromFile method

Belirtilen dosyadaki bir yazı tipini varsayılan olarak kullanarak yeni DocumentFontsSubsystem örneği oluşturun.

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromFile(string filePath, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| filePath | String | Varsayılan yazı tipi adını içeren dosya. |
| fontsSubstitutions | Dictionary`2 | Yazı tipi değişiklikleri. |

### Geri dönüş değeri

[`DocumentFontsSubsystem`](../) .

### Örnekler

Bir dosyadan varsayılan yazı tipini kullanarak bir belgeyi pdf biçiminde nasıl kaydedeceğinizi gösterir.

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

### Ayrıca bakınız

* class [DocumentFontsSubsystem](../)
* ad alanı [Aspose.Note.Fonts](../../documentfontssubsystem/)
* toplantı [Aspose.Note](../../../)


