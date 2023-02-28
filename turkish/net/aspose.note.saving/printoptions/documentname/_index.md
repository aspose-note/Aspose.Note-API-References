---
title: PrintOptions.DocumentName
second_title: Aspose.Note for .NET API Referansı
description: PrintOptions mülk. Belgeyi yazdırırken görüntülenecek örneğin bir yazdırma durumu iletişim kutusunda veya yazıcı kuyruğunda belge adını alır veya ayarlar.
type: docs
weight: 20
url: /tr/net/aspose.note.saving/printoptions/documentname/
---
## PrintOptions.DocumentName property

Belgeyi yazdırırken görüntülenecek (örneğin, bir yazdırma durumu iletişim kutusunda veya yazıcı kuyruğunda) belge adını alır veya ayarlar.

```csharp
public string DocumentName { get; set; }
```

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


