---
title: RevisionSummary.AuthorMostRecent
second_title: Aspose.Note untuk Referensi .NET API
description: RevisionSummary Properti. Mendapat atau menetapkan penulis terbaru.
type: docs
weight: 20
url: /id/net/aspose.note/revisionsummary/authormostrecent/
---
## RevisionSummary.AuthorMostRecent property

Mendapat atau menetapkan penulis terbaru.

```csharp
public string AuthorMostRecent { get; set; }
```

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

* class [RevisionSummary](../)
* ruang nama [Aspose.Note](../../revisionsummary/)
* perakitan [Aspose.Note](../../../)


