---
title: Image.OriginalWidth
second_title: Aspose.Note for .NET API Referansı
description: Image mülk. Orijinal genişliği alır. Bu resmin yeniden boyutlandırmadan önceki orijinal genişliğidir.
type: docs
weight: 150
url: /tr/net/aspose.note/image/originalwidth/
---
## Image.OriginalWidth property

Orijinal genişliği alır. Bu, resmin yeniden boyutlandırmadan önceki orijinal genişliğidir.

```csharp
public float OriginalWidth { get; }
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


