---
title: RichText.Tags
second_title: Aspose.Note for .NET API Referansı
description: RichText mülk. Bir paragrafın tüm etiketlerinin listesini alır.
type: docs
weight: 90
url: /tr/net/aspose.note/richtext/tags/
---
## RichText.Tags property

Bir paragrafın tüm etiketlerinin listesini alır.

```csharp
public List<ITag> Tags { get; }
```

### Örnekler

Outlook görevlerinin ayrıntılarına nasıl erişileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Tasks();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

// Tüm RichText düğümlerini al
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Her düğümü yinele
foreach (RichText richText in nodes)
{
    var tasks = richText.Tags.OfType<NoteTask>();
    if (tasks.Any())
    {
        Console.WriteLine($"Task: {richText.Text}");
        foreach (var noteTask in tasks)
        {
            // özellikleri al
            Console.WriteLine($"    Completed Time: {noteTask.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTask.CreationTime}");
            Console.WriteLine($"    Due Date: {noteTask.DueDate}");
            Console.WriteLine($"    Status: {noteTask.Status}");
            Console.WriteLine($"    Icon: {noteTask.Icon}");
        }
    }
}
```

### Ayrıca bakınız

* interface [ITag](../../itag/)
* class [RichText](../)
* ad alanı [Aspose.Note](../../richtext/)
* toplantı [Aspose.Note](../../../)


