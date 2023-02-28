---
title: Document.GetPageHistory
second_title: Aspose.Note untuk Referensi .NET API
description: Document metode. MendapatkanPageHistory yang berisi riwayat lengkap untuk setiap halaman yang disajikan dalam dokumen paling awal di indeks 0. Revisi halaman saat ini dapat diakses sebagaiCurrent dan terkandung secara terpisah dari kumpulan versi historis.
type: docs
weight: 100
url: /id/net/aspose.note/document/getpagehistory/
---
## Document.GetPageHistory method

Mendapatkan[`PageHistory`](../../pagehistory/) yang berisi riwayat lengkap untuk setiap halaman yang disajikan dalam dokumen (paling awal di indeks 0). Revisi halaman saat ini dapat diakses sebagai[`Current`](../../pagehistory/current/) dan terkandung secara terpisah dari kumpulan versi historis.

```csharp
public PageHistory GetPageHistory(Page page)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| page | Page | Revisi halaman saat ini. |

### Nilai Pengembalian

Itu[`PageHistory`](../../pagehistory/) .

### Contoh

Menunjukkan cara mengembalikan versi halaman sebelumnya.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Pages();

// Muat dokumen OneNote dan dapatkan anak pertama           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;           
Page previousPageVersion = document.GetPageHistory(page).Last();

document.RemoveChild(page);
document.AppendChildLast(previousPageVersion);

document.Save(dataDir + "RollBackRevisions_out.one");
```

Menunjukkan cara mengedit riwayat halaman.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Pages();

// Muat dokumen OneNote dan dapatkan anak pertama           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.RemoveRange(0, 1);

pageHistory[0] = new Page(document);
if (pageHistory.Count > 1)
{
    pageHistory[1].Title.TitleText.Text = "New Title";

    pageHistory.Add(new Page(document));

    pageHistory.Insert(1, new Page(document));

    document.Save(dataDir + "ModifyPageHistory_out.one");
}
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

* class [PageHistory](../../pagehistory/)
* class [Page](../../page/)
* class [Document](../)
* ruang nama [Aspose.Note](../../document/)
* perakitan [Aspose.Note](../../../)


