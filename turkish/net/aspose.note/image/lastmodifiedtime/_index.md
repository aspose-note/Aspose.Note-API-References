---
title: Image.LastModifiedTime
second_title: Aspose.Note for .NET API Referansı
description: Image mülk. Son değiştirilme zamanını alır veya ayarlar.
type: docs
weight: 130
url: /tr/net/aspose.note/image/lastmodifiedtime/
---
## Image.LastModifiedTime property

Son değiştirilme zamanını alır veya ayarlar.

```csharp
public DateTime LastModifiedTime { get; set; }
```

### Örnekler

Görüntünün meta bilgilerinin nasıl alınacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Images();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

// Tüm Görüntü düğümlerini al
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

### Ayrıca bakınız

* class [Image](../)
* ad alanı [Aspose.Note](../../image/)
* toplantı [Aspose.Note](../../../)


