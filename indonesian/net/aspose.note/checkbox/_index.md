---
title: Class CheckBox
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.CheckBox kelas. Kelas dasar untuk tag yang dapat mengalihkan statusnya antara lengkap dan tidak lengkap.
type: docs
weight: 20
url: /id/net/aspose.note/checkbox/
---
## CheckBox class

Kelas dasar untuk tag yang dapat mengalihkan statusnya antara lengkap dan tidak lengkap.

```csharp
public abstract class CheckBox : ITag
```

## Properti

| Nama | Keterangan |
| --- | --- |
| [Checked](../../aspose.note/checkbox/checked/) { get; } | Mendapat nilai yang menunjukkan apakah Kotak Centang dalam keadaan dicentang. |
| [CompletedTime](../../aspose.note/checkbox/completedtime/) { get; } | Mendapat atau menyetel waktu selesai. |
| [CreationTime](../../aspose.note/checkbox/creationtime/) { get; set; } | Mendapatkan atau menyetel waktu pembuatan. |
| abstract [Icon](../../aspose.note/checkbox/icon/) { get; } | Mendapat atau menyetel ikon. |
| [Label](../../aspose.note/checkbox/label/) { get; } | Mendapat teks label. |
| [Status](../../aspose.note/checkbox/status/) { get; } | Mendapat atau menyetel status. |

## Metode

| Nama | Keterangan |
| --- | --- |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/#setcompleted)() | Menyetel tag ke status selesai menggunakan waktu saat ini sebagai waktu selesai. |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/#setcompleted_1)(DateTime) | Menyetel tag ke status selesai. |
| virtual [SetOpen](../../aspose.note/checkbox/setopen/)() | Mengatur tag ke status terbuka. |

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

Menunjukkan cara menyelesaikan semua item kotak centang yang terkait dengan 'Proyek C'.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Tags();

// Muat dokumen ke Aspose.Note.
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

Menunjukkan cara membuka semua item kotak centang yang terkait dengan 'Project C'.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Tags();

// Muat dokumen ke Aspose.Note.
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

Menunjukkan cara membuat pdf yang berisi halaman dengan item yang ditandai dengan kotak centang tidak lengkap dan dibuat selama minggu lalu.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Tags();

// Muat dokumen ke Aspose.Note.
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

Menunjukkan cara membuat pdf yang berisi halaman dengan tugas Outlook yang belum selesai untuk diselesaikan pada minggu ini.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Tags();

// Muat dokumen ke Aspose.Note.
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

### Lihat juga

* interface [ITag](../itag/)
* ruang nama [Aspose.Note](../../aspose.note/)
* perakitan [Aspose.Note](../../)


