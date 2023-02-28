---
title: Page.LastModifiedTime
second_title: Aspose.Note untuk Referensi .NET API
description: Page Properti. Mendapatkan atau menyetel waktu modifikasi terakhir.
type: docs
weight: 60
url: /id/net/aspose.note/page/lastmodifiedtime/
---
## Page.LastModifiedTime property

Mendapatkan atau menyetel waktu modifikasi terakhir.

```csharp
public DateTime LastModifiedTime { get; set; }
```

### Contoh

Menunjukkan cara mendapatkan informasi meta tentang suatu halaman.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Pages();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

foreach (Page page in oneFile)
{
    Console.WriteLine("LastModifiedTime: {0}", page.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", page.CreationTime);
    Console.WriteLine("Title: {0}", page.Title);
    Console.WriteLine("Level: {0}", page.Level);
    Console.WriteLine("Author: {0}", page.Author);
    Console.WriteLine();
}
```

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

* class [Page](../)
* ruang nama [Aspose.Note](../../page/)
* perakitan [Aspose.Note](../../../)


