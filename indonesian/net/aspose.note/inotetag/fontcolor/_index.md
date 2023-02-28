---
title: INoteTag.FontColor
second_title: Aspose.Note untuk Referensi .NET API
description: INoteTag Properti. Mendapat atau mengatur warna font.
type: docs
weight: 10
url: /id/net/aspose.note/inotetag/fontcolor/
---
## INoteTag.FontColor property

Mendapat atau mengatur warna font.

```csharp
public Color FontColor { get; set; }
```

### Contoh

Menunjukkan cara mengakses detail tag.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Tags();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "TagFile.one");

// Dapatkan semua node RichText
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Iterasi melalui setiap node
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // Ambil properti
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

### Lihat juga

* interface [INoteTag](../)
* ruang nama [Aspose.Note](../../inotetag/)
* perakitan [Aspose.Note](../../../)


