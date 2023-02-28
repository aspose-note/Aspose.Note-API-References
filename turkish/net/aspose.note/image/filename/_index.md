---
title: Image.FileName
second_title: Aspose.Note for .NET API Referansı
description: Image mülk. Dosya adını alır.
type: docs
weight: 60
url: /tr/net/aspose.note/image/filename/
---
## Image.FileName property

Dosya adını alır.

```csharp
public string FileName { get; }
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


