---
title: ITag
second_title: Aspose.Note for .NET API Referansı
description: Her türden etiket için arayüz.
type: docs
weight: 220
url: /tr/net/aspose.note/itag/
---
## ITag interface

Her türden etiket için arayüz.

```csharp
public interface ITag
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [CompletedTime](../../aspose.note/itag/completedtime) { get; } | Tamamlanan zamanı alır veya ayarlar. |
| [CreationTime](../../aspose.note/itag/creationtime) { get; set; } | Oluşturma zamanını alır veya ayarlar. |
| [Icon](../../aspose.note/itag/icon) { get; } | Simgeyi alır veya ayarlar. |
| [Label](../../aspose.note/itag/label) { get; } | Etiket metnini alır. |
| [Status](../../aspose.note/itag/status) { get; } | Durumu alır veya ayarlar. |

### Örnekler

'Proje A' ile ilgili tüm sayfaları içeren bir pdf'nin nasıl oluşturulacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Tags();

// Belgeyi Aspose.Note'a yükleyin.
var oneFile = new Document(Path.Combine(dataDir, "ProjectNotes.one"));

var report = new Document();
foreach (var page in oneFile)
{
    if (page.GetChildNodes<ITaggable>().Any(e => e.Tags.Any(x => x.Label.Contains("Project A"))))
    {
        report.AppendChildLast(page.Clone());
    }
}

report.Save(Path.Combine(dataDir, "ProjectA_Report.pdf"));
```

'Proje C' ile ilgili tüm onay kutusu öğelerinin nasıl tamamlanacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Tags();

// Belgeyi Aspose.Note'a yükleyin.
var oneFile = new Document(Path.Combine(dataDir, "ProjectNotes.one"));

foreach (var node in oneFile.GetChildNodes<ITaggable>())
{
    foreach (var checkBox in node.Tags.OfType<CheckBox>())
    {
        if (checkBox.Label.Contains("Project C") && !checkBox.Checked)
        {
            checkBox.SetCompleted();
        }
    }
}

oneFile.Save(Path.Combine(dataDir, ClosedProjectCNotesFileName));
```

'Proje C' ile ilgili tüm onay kutusu öğelerinin nasıl açılacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Tags();

// Belgeyi Aspose.Note'a yükleyin.
var oneFile = new Document(Path.Combine(dataDir, ClosedProjectCNotesFileName));

foreach (var node in oneFile.GetChildNodes<ITaggable>())
{
    foreach (var checkBox in node.Tags.OfType<CheckBox>())
    {
        if (checkBox.Label.Contains("Project C") && checkBox.Checked)
        {
            checkBox.SetOpen();
        }
    }
}

oneFile.Save(Path.Combine(dataDir, "ProjectNoteWithOpenProjectC.one"));
```

Eksik onay kutuları ile işaretlenmiş ve geçen hafta oluşturulmuş öğeler içeren sayfaları içeren bir pdf'nin nasıl oluşturulacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Tags();

// Belgeyi Aspose.Note'a yükleyin.
var oneFile = new Document(Path.Combine(dataDir, "TagFile.one"));

var report = new Document();
foreach (var page in oneFile)
{
    if (page.GetChildNodes<ITaggable>().Any(e => e.Tags.OfType<CheckBox>().Any(x => !x.Checked && DateTime.UtcNow.Subtract(TimeSpan.FromDays(7)) <= x.CreationTime)))
    {
        report.AppendChildLast(page.Clone());
    }
}

report.Save(Path.Combine(dataDir, "IncompleteLastWeekReport.pdf"));
```

Bu hafta tamamlanacak Outlook'un tamamlanmamış görevleri olan sayfaları içeren bir pdf'nin nasıl oluşturulacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Tags();

// Belgeyi Aspose.Note'a yükleyin.
var oneFile = new Document(Path.Combine(dataDir, "TagFile.one"));

var report = new Document();
var endOfWeek = DateTime.Today.AddDays(5 - (int)DateTime.Today.DayOfWeek);
foreach (var page in oneFile)
{
    if (page.GetChildNodes<ITaggable>().Any(e => e.Tags.OfType<NoteTask>().Any(x => !x.Checked && DateTime.UtcNow.Subtract(TimeSpan.FromDays(7)) <= x.CreationTime && x.DueDate <= endOfWeek)))
    {
        report.AppendChildLast(page.Clone());
    }
}

report.Save(Path.Combine(dataDir, "IncompleteTasksForThisWeekReport.pdf"));
```

Outlook'un görevlerinin ayrıntılarına nasıl erişileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Tasks();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

// Tüm RichText düğümlerini al
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Her düğümde yineleme
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

Bir etiketin ayrıntılarına nasıl erişileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Tags();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "TagFile.one");

// Tüm RichText düğümlerini al
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Her düğümde yineleme
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

* ad alanı [Aspose.Note](../../aspose.note)
* toplantı [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
