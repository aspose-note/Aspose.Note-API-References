---
title: Image.Bytes
second_title: Aspose.Note for .NET API Referansı
description: Image mülk. Görüntü veri deposunu alır.
type: docs
weight: 50
url: /tr/net/aspose.note/image/bytes/
---
## Image.Bytes property

Görüntü veri deposunu alır.

```csharp
public byte[] Bytes { get; }
```

### Örnekler

Bir belgeden nasıl resim alınacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Images();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

// Tüm Görüntü düğümlerini al
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Görüntü baytlarını bir dosyaya kaydet
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

### Ayrıca bakınız

* class [Image](../)
* ad alanı [Aspose.Note](../../image/)
* toplantı [Aspose.Note](../../../)


