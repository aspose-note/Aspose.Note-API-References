---
title: RichText.Tags
second_title: Aspose.Note untuk Referensi .NET API
description: RichText Properti. Mendapat daftar semua tag paragraf.
type: docs
weight: 90
url: /id/net/aspose.note/richtext/tags/
---
## RichText.Tags property

Mendapat daftar semua tag paragraf.

```csharp
public List<ITag> Tags { get; }
```

### Contoh

Menunjukkan cara mengakses detail tugas Outlook.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Tasks();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Dapatkan semua node RichText
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Iterasi melalui setiap node
foreach (RichText richText in nodes)
{
    var tasks = richText.Tags.OfType<NoteTask>();
    if (tasks.Any())
    {
        Console.WriteLine($"Task: {richText.Text}");
        foreach (var noteTask in tasks)
        {
            // Ambil properti
            Console.WriteLine($"    Completed Time: {noteTask.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTask.CreationTime}");
            Console.WriteLine($"    Due Date: {noteTask.DueDate}");
            Console.WriteLine($"    Status: {noteTask.Status}");
            Console.WriteLine($"    Icon: {noteTask.Icon}");
        }
    }
}
```

### Lihat juga

* interface [ITag](../../itag/)
* class [RichText](../)
* ruang nama [Aspose.Note](../../richtext/)
* perakitan [Aspose.Note](../../../)


