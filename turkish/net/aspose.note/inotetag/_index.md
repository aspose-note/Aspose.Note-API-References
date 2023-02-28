---
title: Interface INoteTag
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.INoteTag arayüz. Not etiketleri için arabirim yani Outlook görevleriyle ilişkili olmayan etiketler.
type: docs
weight: 180
url: /tr/net/aspose.note/inotetag/
---
## INoteTag interface

Not etiketleri için arabirim (yani, Outlook görevleriyle ilişkili olmayan etiketler).

```csharp
public interface INoteTag : ITag
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [FontColor](../../aspose.note/inotetag/fontcolor/) { get; set; } | Yazı tipi rengini alır veya ayarlar. |
| [Highlight](../../aspose.note/inotetag/highlight/) { get; set; } | Vurgu rengini alır veya ayarlar. |
| [Label](../../aspose.note/inotetag/label/) { get; set; } | Etiket metnini alır veya ayarlar. |

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

* interface [ITag](../itag/)
* ad alanı [Aspose.Note](../../aspose.note/)
* toplantı [Aspose.Note](../../)


