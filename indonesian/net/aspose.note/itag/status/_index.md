---
title: ITag.Status
second_title: Aspose.Note untuk Referensi .NET API
description: ITag Properti. Mendapat atau menyetel status.
type: docs
weight: 50
url: /id/net/aspose.note/itag/status/
---
## ITag.Status property

Mendapat atau menyetel status.

```csharp
public TagStatus Status { get; }
```

### Nilai properti

Itu[`TagStatus`](../../tagstatus/) .

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

* enum [TagStatus](../../tagstatus/)
* interface [ITag](../)
* ruang nama [Aspose.Note](../../itag/)
* perakitan [Aspose.Note](../../../)


