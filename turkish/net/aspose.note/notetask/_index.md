---
title: Class NoteTask
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.NoteTask sınıf. Bir not görevini temsil eder.
type: docs
weight: 400
url: /tr/net/aspose.note/notetask/
---
## NoteTask class

Bir not görevini temsil eder.

```csharp
public sealed class NoteTask : CheckBox, IEquatable<NoteTask>
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Checked](../../aspose.note/checkbox/checked/) { get; } | CheckBox'ın kontrol edilmiş durumda olup olmadığını gösteren bir değer alır. |
| [CompletedTime](../../aspose.note/checkbox/completedtime/) { get; } | Tamamlanan süreyi alır veya ayarlar. |
| [CreationTime](../../aspose.note/checkbox/creationtime/) { get; set; } | Oluşturma zamanını alır veya ayarlar. |
| [DueDate](../../aspose.note/notetask/duedate/) { get; set; } | Bitiş tarihini alır veya ayarlar. |
| override [Icon](../../aspose.note/notetask/icon/) { get; } | Simgeyi alır veya ayarlar. |
| [Label](../../aspose.note/checkbox/label/) { get; } | Etiket metnini alır. |
| [Status](../../aspose.note/checkbox/status/) { get; } | Durumu alır veya ayarlar. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| static [CreateCustomFollowUpDate](../../aspose.note/notetask/createcustomfollowupdate/)(DateTime) | NoFollowUpDateFlag simgesi ve belirtilen teslim tarihi ile yeni bir not görevi oluşturur. |
| static [CreateFollowUpNextWeek](../../aspose.note/notetask/createfollowupnextweek/)() | FollowUpNextWeekFlag simgesiyle yeni bir not görevi oluşturur. |
| static [CreateFollowUpThisWeek](../../aspose.note/notetask/createfollowupthisweek/)() | FollowUpThisWeekFlag simgesiyle yeni bir not görevi oluşturur. |
| static [CreateFollowUpToday](../../aspose.note/notetask/createfollowuptoday/)() | FollowUpTodayFlag simgesiyle yeni bir not görevi oluşturur. |
| static [CreateFollowUpTomorrow](../../aspose.note/notetask/createfollowuptomorrow/)() | FollowUpTomorrowFlag simgesiyle yeni bir not görevi oluşturur. |
| static [CreateNoFollowUpDate](../../aspose.note/notetask/createnofollowupdate/)() | NoFollowUpDateFlag simgesiyle yeni bir not görevi oluşturur. |
| [Equals](../../aspose.note/notetask/equals/#equals)(NoteTask) | Belirtilen nesnenin geçerli nesneye eşit olup olmadığını belirler. |
| override [Equals](../../aspose.note/notetask/equals/#equals_1)(object) | Belirtilen nesnenin geçerli nesneye eşit olup olmadığını belirler. |
| override [GetHashCode](../../aspose.note/notetask/gethashcode/)() | type. için bir hash işlevi olarak hizmet eder |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/)() | Geçerli saati tamamlanma süresi olarak kullanarak etiketi tamamlanmış duruma ayarlar. |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/)(DateTime) | Etiketi tamamlanmış duruma ayarlar. |
| override [SetOpen](../../aspose.note/notetask/setopen/)() | Etiketi durumu açacak şekilde ayarlar. |

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

* class [CheckBox](../checkbox/)
* ad alanı [Aspose.Note](../../aspose.note/)
* toplantı [Aspose.Note](../../)


