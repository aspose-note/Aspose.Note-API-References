---
title: Page.IsConflictPage
second_title: Aspose.Note untuk Referensi .NET API
description: Page Properti. Mendapat atau menetapkan nilai yang menunjukkan apakah halaman ini merupakan halaman konflik.
type: docs
weight: 50
url: /id/net/aspose.note/page/isconflictpage/
---
## Page.IsConflictPage property

Mendapat atau menetapkan nilai yang menunjukkan apakah halaman ini merupakan halaman konflik.

```csharp
public bool IsConflictPage { get; set; }
```

### Perkataan

Halaman konflik muncul ketika dua pengguna mencoba memperbarui konten yang sama. Dalam hal ini, perubahan pengguna pertama ditulis seperti biasa. Namun perubahan pengguna lain tidak dapat digabungkan. Jadi hanya salinan halaman yang dibuat dan ditandai sebagai konflik.

Pada versi ini konflik diselesaikan demi perubahan pengguna pertama. Jadi jika dokumen memiliki halaman konflik maka mereka akan ditampilkan dalam riwayat tetapi akan dilewati saat disimpan. Dimungkinkan untuk mengatur ulang bendera ini untuk menyimpan halaman ini dalam sejarah seperti biasa.

Contoh detail halaman manipulasi konflik dapat ditemukan di dokumentasi online.

### Contoh

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

* class [Page](../)
* ruang nama [Aspose.Note](../../page/)
* perakitan [Aspose.Note](../../../)


