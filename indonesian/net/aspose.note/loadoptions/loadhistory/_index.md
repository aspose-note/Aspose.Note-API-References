---
title: LoadOptions.LoadHistory
second_title: Aspose.Note untuk Referensi .NET API
description: LoadOptions Properti. Mendapat atau menetapkan nilai yang menunjukkan apakah pemuat dokumen harus mengabaikan riwayat. Gunakan opsi ini untuk mengurangi penggunaan memori dan CPU. Nilai defaultnya adalahBENAR .
type: docs
weight: 30
url: /id/net/aspose.note/loadoptions/loadhistory/
---
## LoadOptions.LoadHistory property

Mendapat atau menetapkan nilai yang menunjukkan apakah pemuat dokumen harus mengabaikan riwayat. Gunakan opsi ini untuk mengurangi penggunaan memori dan CPU. Nilai defaultnya adalah`BENAR` .

```csharp
public bool LoadHistory { get; set; }
```

### Contoh

Menunjukkan cara mendapatkan riwayat halaman.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Pages();

// Muat dokumen OneNote
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Dapatkan halaman pertama
Page firstPage = document.FirstChild;
foreach (Page pageRevision in document.GetPageHistory(firstPage))
{
    /*Use pageRevision like a regular page.*/
    Console.WriteLine("LastModifiedTime: {0}", pageRevision.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", pageRevision.CreationTime);
    Console.WriteLine("Title: {0}", pageRevision.Title);
    Console.WriteLine("Level: {0}", pageRevision.Level);
    Console.WriteLine("Author: {0}", pageRevision.Author);
    Console.WriteLine();
}
```

### Lihat juga

* class [LoadOptions](../)
* ruang nama [Aspose.Note](../../loadoptions/)
* perakitan [Aspose.Note](../../../)


