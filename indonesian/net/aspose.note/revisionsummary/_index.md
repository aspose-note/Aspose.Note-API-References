---
title: Class RevisionSummary
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.RevisionSummary kelas. Merupakan ringkasan untuk revisi node.
type: docs
weight: 520
url: /id/net/aspose.note/revisionsummary/
---
## RevisionSummary class

Merupakan ringkasan untuk revisi node.

```csharp
public class RevisionSummary
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [RevisionSummary](revisionsummary/)() | Konstruktor default. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [AuthorMostRecent](../../aspose.note/revisionsummary/authormostrecent/) { get; set; } | Mendapat atau menetapkan penulis terbaru. |
| [LastModifiedTime](../../aspose.note/revisionsummary/lastmodifiedtime/) { get; set; } | Mendapatkan atau menyetel waktu modifikasi terakhir. |

### Contoh

Menunjukkan cara mengedit informasi meta halaman.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Pages();

// Muat dokumen OneNote dan dapatkan anak pertama           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

// Membaca Ringkasan Revisi Konten untuk halaman ini
var pageRevisionInfo = page.PageContentRevisionSummary;

Console.WriteLine(string.Format(
    "Author:\t{0}\nModified:\t{1}",
    pageRevisionInfo.AuthorMostRecent,
    pageRevisionInfo.LastModifiedTime.ToString("dd.MM.yyyy HH:mm:ss")));

// Perbarui Ringkasan Revisi Halaman untuk halaman ini
pageRevisionInfo.AuthorMostRecent = "New Author";
pageRevisionInfo.LastModifiedTime = DateTime.Now;

document.Save(dataDir + "WorkingWithPageRevisions_out.one");
```

Memperlihatkan cara memeriksa apakah sebuah halaman adalah halaman konflik (yaitu ada perubahan yang tidak dapat digabungkan secara otomatis oleh OneNote).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// Muat dokumen OneNote
Document doc = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

var history = doc.GetPageHistory(doc.FirstChild);
for (int i = 0; i < history.Count; i++)
{
    var historyPage = history[i];
    Console.Write("    {0}. Author: {1}, {2:dd.MM.yyyy hh.mm.ss}",
                    i,
                    historyPage.PageContentRevisionSummary.AuthorMostRecent,
                    historyPage.PageContentRevisionSummary.LastModifiedTime);
    Console.WriteLine(historyPage.IsConflictPage ? ", IsConflict: true" : string.Empty);

    // Secara default, halaman konflik dilewati begitu saja saat disimpan.
    // Jika menandainya sebagai non-konflik maka akan disimpan seperti biasanya di riwayat.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

### Lihat juga

* ruang nama [Aspose.Note](../../aspose.note/)
* perakitan [Aspose.Note](../../)


