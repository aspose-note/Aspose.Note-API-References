---
title: Interface INoteTag
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.INoteTag antarmuka. Antarmuka untuk tag catatan yaitu tag yang tidak terkait dengan tugas Outlook.
type: docs
weight: 180
url: /id/net/aspose.note/inotetag/
---
## INoteTag interface

Antarmuka untuk tag catatan (yaitu tag yang tidak terkait dengan tugas Outlook).

```csharp
public interface INoteTag : ITag
```

## Properti

| Nama | Keterangan |
| --- | --- |
| [FontColor](../../aspose.note/inotetag/fontcolor/) { get; set; } | Mendapat atau mengatur warna font. |
| [Highlight](../../aspose.note/inotetag/highlight/) { get; set; } | Mendapat atau menyetel warna sorotan. |
| [Label](../../aspose.note/inotetag/label/) { get; set; } | Mendapat atau menyetel teks label. |

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

* interface [ITag](../itag/)
* ruang nama [Aspose.Note](../../aspose.note/)
* perakitan [Aspose.Note](../../)


