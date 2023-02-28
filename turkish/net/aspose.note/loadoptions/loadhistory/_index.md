---
title: LoadOptions.LoadHistory
second_title: Aspose.Note for .NET API Referansı
description: LoadOptions mülk. Bir belge yükleyicinin geçmişi yok sayması gerekip gerekmediğini belirten bir değer alır veya ayarlar. Bellek ve CPU kullanımını azaltmak için bu seçeneği kullanın. Varsayılan değerdoğru .
type: docs
weight: 30
url: /tr/net/aspose.note/loadoptions/loadhistory/
---
## LoadOptions.LoadHistory property

Bir belge yükleyicinin geçmişi yok sayması gerekip gerekmediğini belirten bir değer alır veya ayarlar. Bellek ve CPU kullanımını azaltmak için bu seçeneği kullanın. Varsayılan değer:`doğru` .

```csharp
public bool LoadHistory { get; set; }
```

### Örnekler

Sayfa geçmişinin nasıl alınacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote belgesini yükleyin
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// İlk sayfayı al
Page firstPage = document.FirstChild;
foreach (Page pageRevision in document.GetPageHistory(firstPage))
{
    /*Use pageRevision like a regular page.*/
    Console.WriteLine("LastModifiedTime: {0}", pageRevision.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", pageRevision.CreationTime);
    Console.WriteLine("Title: {0}", pageRevision.Title);
    Console.WriteLine("Level: {0}", pageRevision.Level);
    Console.WriteLine("Author: {0}", pageRevision.Author);
    Console.WriteLine();
}
```

### Ayrıca bakınız

* class [LoadOptions](../)
* ad alanı [Aspose.Note](../../loadoptions/)
* toplantı [Aspose.Note](../../../)


