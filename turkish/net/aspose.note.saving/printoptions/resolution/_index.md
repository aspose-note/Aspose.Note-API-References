---
title: PrintOptions.Resolution
second_title: Aspose.Note for .NET API Referansı
description: PrintOptions mülk. Oluşturulan görüntülerin çözünürlüğünü inç başına nokta cinsinden alır veya ayarlar.
type: docs
weight: 50
url: /tr/net/aspose.note.saving/printoptions/resolution/
---
## PrintOptions.Resolution property

Oluşturulan görüntülerin çözünürlüğünü inç başına nokta cinsinden alır veya ayarlar.

```csharp
public float Resolution { get; set; }
```

### Notlar

Varsayılan değer 96. 'dir.

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

* class [PrintOptions](../)
* ad alanı [Aspose.Note.Saving](../../printoptions/)
* toplantı [Aspose.Note](../../../)


