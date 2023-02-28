---
title: Document.DetectLayoutChanges
second_title: Aspose.Note for .NET API Referansı
description: Document yöntem. Öncekinden bu yana belge düzeninde yapılan tüm değişiklikleri algılar.DetectLayoutChanges call. DurumdaAutomaticLayoutChangesDetectionEnabled true olarak ayarlandı belge dışa aktarımının başlangıcında otomatik olarak kullanıldı.
type: docs
weight: 90
url: /tr/net/aspose.note/document/detectlayoutchanges/
---
## Document.DetectLayoutChanges method

Öncekinden bu yana belge düzeninde yapılan tüm değişiklikleri algılar.`DetectLayoutChanges` call. Durumda[`AutomaticLayoutChangesDetectionEnabled`](../automaticlayoutchangesdetectionenabled/) true olarak ayarlandı, belge dışa aktarımının başlangıcında otomatik olarak kullanıldı.

```csharp
public void DetectLayoutChanges()
```

### Örnekler

Bir belgenin farklı biçimlerde nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Yeni Belgeyi başlat
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// Yeni Sayfayı başlat
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Belgedeki tüm metin için varsayılan stil.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Sayfa düğümünü ekle
doc.AppendChildLast(page);

// OneNote belgesini farklı biçimlerde kaydedin, metin yazı tipi boyutunu ayarlayın ve düzen değişikliklerini manuel olarak algılayın.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

### Ayrıca bakınız

* class [Document](../)
* ad alanı [Aspose.Note](../../document/)
* toplantı [Aspose.Note](../../../)


