---
title: Interface ITaggable
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.ITaggable antarmuka. Antarmuka untuk node yang dapat ditandai dengan tag.
type: docs
weight: 240
url: /id/net/aspose.note/itaggable/
---
## ITaggable interface

Antarmuka untuk node yang dapat ditandai dengan tag.

```csharp
public interface ITaggable : INode
```

## Properti

| Nama | Keterangan |
| --- | --- |
| [Tags](../../aspose.note/itaggable/tags/) { get; } | Mendapat daftar semua tag. |

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

* interface [INode](../inode/)
* ruang nama [Aspose.Note](../../aspose.note/)
* perakitan [Aspose.Note](../../)


