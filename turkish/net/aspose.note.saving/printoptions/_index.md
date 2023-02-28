---
title: Class PrintOptions
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.Saving.PrintOptions sınıf. Bir belgeyi yazdırmak için kullanılan seçenekler.
type: docs
weight: 860
url: /tr/net/aspose.note.saving/printoptions/
---
## PrintOptions class

Bir belgeyi yazdırmak için kullanılan seçenekler.

```csharp
public class PrintOptions
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [PrintOptions](printoptions/)() | Default_Constructor |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [DocumentName](../../aspose.note.saving/printoptions/documentname/) { get; set; } | Belgeyi yazdırırken görüntülenecek (örneğin, bir yazdırma durumu iletişim kutusunda veya yazıcı kuyruğunda) belge adını alır veya ayarlar. |
| [PageSplittingAlgorithm](../../aspose.note.saving/printoptions/pagesplittingalgorithm/) { get; set; } | Sayfa bölme için kullanılan algoritmayı alır veya ayarlar. |
| [PrinterSettings](../../aspose.note.saving/printoptions/printersettings/) { get; set; } | Yazıcı ayarlarını alır veya ayarlar. |
| [Resolution](../../aspose.note.saving/printoptions/resolution/) { get; set; } | Oluşturulan görüntülerin çözünürlüğünü inç başına nokta cinsinden alır veya ayarlar. |

### Örnekler

Belirtilen seçeneklerle standart Windows iletişim kutusunu kullanarak belgenin bir yazıcıya nasıl gönderileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

var printerSettings = new PrinterSettings() { FromPage = 0, ToPage = 10 };
printerSettings.DefaultPageSettings.Landscape = true;
printerSettings.DefaultPageSettings.Margins = new System.Drawing.Printing.Margins(50, 50, 150, 50);

document.Print(new PrintOptions()
               {
                   PrinterSettings = printerSettings,
                   Resolution = 1200,
                   PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(),
                   DocumentName = "Test.one"
               });
```

### Ayrıca bakınız

* ad alanı [Aspose.Note.Saving](../../aspose.note.saving/)
* toplantı [Aspose.Note](../../)


