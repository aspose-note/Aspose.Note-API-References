---
title: INoteTag.Highlight
second_title: Aspose.Note for .NET API Referansı
description: INoteTag mülk. Vurgu rengini alır veya ayarlar.
type: docs
weight: 20
url: /tr/net/aspose.note/inotetag/highlight/
---
## INoteTag.Highlight property

Vurgu rengini alır veya ayarlar.

```csharp
public Color Highlight { get; set; }
```

### Örnekler

Bir etiketin ayrıntılarına nasıl erişileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Tags();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "TagFile.one");

// Tüm RichText düğümlerini al
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Her düğümü yinele
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // özellikleri al
            Console.WriteLine($"    Completed Time: {noteTag.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTag.CreationTime}");
            Console.WriteLine($"    Font Color: {noteTag.FontColor}");
            Console.WriteLine($"    Status: {noteTag.Status}");
            Console.WriteLine($"    Label: {noteTag.Label}");
            Console.WriteLine($"    Icon: {noteTag.Icon}");
            Console.WriteLine($"    High Light: {noteTag.Highlight}");
        }
    }
}
```

### Ayrıca bakınız

* interface [INoteTag](../)
* ad alanı [Aspose.Note](../../inotetag/)
* toplantı [Aspose.Note](../../../)


