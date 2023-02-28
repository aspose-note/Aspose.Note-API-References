---
title: PageSettings.Letter
second_title: Aspose.Note untuk Referensi .NET API
description: PageSettings Properti. Mendapat pengaturan untuk halaman format Surat.
type: docs
weight: 30
url: /id/net/aspose.note.saving/pagesettings/letter/
---
## PageSettings.Letter property

Mendapat pengaturan untuk halaman format Surat.

```csharp
public static PageSettings Letter { get; }
```

### Contoh

Menunjukkan cara menyimpan dokumen dalam format Pdf dengan tata letak halaman Surat.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// Simpan dokumen.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

### Lihat juga

* class [PageSettings](../)
* ruang nama [Aspose.Note.Saving](../../pagesettings/)
* perakitan [Aspose.Note](../../../)


