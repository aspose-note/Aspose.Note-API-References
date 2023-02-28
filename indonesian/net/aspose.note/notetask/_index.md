---
title: Class NoteTask
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.NoteTask kelas. Merupakan tugas catatan.
type: docs
weight: 400
url: /id/net/aspose.note/notetask/
---
## NoteTask class

Merupakan tugas catatan.

```csharp
public sealed class NoteTask : CheckBox, IEquatable<NoteTask>
```

## Properti

| Nama | Keterangan |
| --- | --- |
| [Checked](../../aspose.note/checkbox/checked/) { get; } | Mendapat nilai yang menunjukkan apakah Kotak Centang dalam keadaan dicentang. |
| [CompletedTime](../../aspose.note/checkbox/completedtime/) { get; } | Mendapat atau menyetel waktu selesai. |
| [CreationTime](../../aspose.note/checkbox/creationtime/) { get; set; } | Mendapatkan atau menyetel waktu pembuatan. |
| [DueDate](../../aspose.note/notetask/duedate/) { get; set; } | Mendapat atau mengatur tanggal jatuh tempo. |
| override [Icon](../../aspose.note/notetask/icon/) { get; } | Mendapat atau menyetel ikon. |
| [Label](../../aspose.note/checkbox/label/) { get; } | Mendapat teks label. |
| [Status](../../aspose.note/checkbox/status/) { get; } | Mendapat atau menyetel status. |

## Metode

| Nama | Keterangan |
| --- | --- |
| static [CreateCustomFollowUpDate](../../aspose.note/notetask/createcustomfollowupdate/)(DateTime) | Membuat tugas catatan baru dengan ikon NoFollowUpDateFlag dan tanggal jatuh tempo yang ditentukan. |
| static [CreateFollowUpNextWeek](../../aspose.note/notetask/createfollowupnextweek/)() | Membuat tugas catatan baru dengan ikon FollowUpNextWeekFlag. |
| static [CreateFollowUpThisWeek](../../aspose.note/notetask/createfollowupthisweek/)() | Membuat tugas catatan baru dengan ikon FollowUpThisWeekFlag. |
| static [CreateFollowUpToday](../../aspose.note/notetask/createfollowuptoday/)() | Membuat tugas catatan baru dengan ikon FollowUpTodayFlag. |
| static [CreateFollowUpTomorrow](../../aspose.note/notetask/createfollowuptomorrow/)() | Membuat tugas catatan baru dengan ikon FollowUpTomorrowFlag. |
| static [CreateNoFollowUpDate](../../aspose.note/notetask/createnofollowupdate/)() | Membuat tugas catatan baru dengan ikon NoFollowUpDateFlag. |
| [Equals](../../aspose.note/notetask/equals/#equals)(NoteTask) | Menentukan apakah objek yang ditentukan sama dengan objek saat ini. |
| override [Equals](../../aspose.note/notetask/equals/#equals_1)(object) | Menentukan apakah objek yang ditentukan sama dengan objek saat ini. |
| override [GetHashCode](../../aspose.note/notetask/gethashcode/)() | Berfungsi sebagai fungsi hash untuk tipe. |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/)() | Menyetel tag ke status selesai menggunakan waktu saat ini sebagai waktu selesai. |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/)(DateTime) | Menyetel tag ke status selesai. |
| override [SetOpen](../../aspose.note/notetask/setopen/)() | Mengatur tag ke status terbuka. |

### Contoh

Menunjukkan cara menghasilkan pdf yang berisi semua halaman yang terkait dengan 'Proyek A'.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Tags();

// Muat dokumen ke Aspose.Note.
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

* class [CheckBox](../checkbox/)
* ruang nama [Aspose.Note](../../aspose.note/)
* perakitan [Aspose.Note](../../)


