---
title: AttachedFile.Bytes
second_title: Aspose.Note for .NET API Referansı
description: AttachedFile mülk. Katıştırılmış bir dosya için ikili verileri alır.
type: docs
weight: 50
url: /tr/net/aspose.note/attachedfile/bytes/
---
## AttachedFile.Bytes property

Katıştırılmış bir dosya için ikili verileri alır.

```csharp
public byte[] Bytes { get; }
```

### Örnekler

Ekli bir dosyanın içeriğinin nasıl alınacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Attachments();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Sample1.one");

// Ekli dosya düğümlerinin bir listesini alın
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// Tüm düğümleri yinele
foreach (AttachedFile file in nodes)
{
    // Ekli dosyayı bir akış nesnesine yükleyin
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // Yerel bir dosya oluştur
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // Dosya akışını kopyala
            CopyStream(outputStream, fileStream);
        }
    }
}
```

### Ayrıca bakınız

* class [AttachedFile](../)
* ad alanı [Aspose.Note](../../attachedfile/)
* toplantı [Aspose.Note](../../../)


