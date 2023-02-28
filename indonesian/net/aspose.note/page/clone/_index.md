---
title: Page.Clone
second_title: Aspose.Note untuk Referensi .NET API
description: Page metode. Menggandakan halaman.
type: docs
weight: 140
url: /id/net/aspose.note/page/clone/
---
## Page.Clone method

Menggandakan halaman.

```csharp
public Page Clone(bool cloneHistory = false)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| cloneHistory | Boolean | Menentukan apakah riwayat halaman harus digandakan.. |

### Nilai Pengembalian

Sebuah tiruan dari halaman.

### Contoh

Menunjukkan cara mendorong versi laman saat ini ke riwayat.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Pages();

// Muat dokumen OneNote dan dapatkan anak pertama           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.Add(page.Clone());

document.Save(dataDir + "PushCurrentPageVersion_out.one");
```

Menunjukkan cara mengkloning halaman.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Pages();

// Muat dokumen OneNote
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Kloning ke dokumen baru tanpa riwayat
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// Klon ke dokumen baru dengan sejarah
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

### Lihat juga

* class [Page](../)
* ruang nama [Aspose.Note](../../page/)
* perakitan [Aspose.Note](../../../)


