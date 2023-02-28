---
title: Class PageSettings
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.Saving.PageSettings kelas. Mewakili pengaturan tata letak halaman.
type: docs
weight: 820
url: /id/net/aspose.note.saving/pagesettings/
---
## PageSettings class

Mewakili pengaturan tata letak halaman.

```csharp
public class PageSettings
```

## Properti

| Nama | Keterangan |
| --- | --- |
| static [A4](../../aspose.note.saving/pagesettings/a4/) { get; } | Mendapat pengaturan untuk halaman format A4. |
| static [A4NoHeightLimit](../../aspose.note.saving/pagesettings/a4noheightlimit/) { get; } | Mendapat pengaturan untuk halaman format A4 dengan ketinggian tak terbatas. |
| static [Letter](../../aspose.note.saving/pagesettings/letter/) { get; } | Mendapat pengaturan untuk halaman format Surat. |
| static [LetterNoHeightLimit](../../aspose.note.saving/pagesettings/letternoheightlimit/) { get; } | Mendapat pengaturan untuk halaman format Surat dengan tinggi tak terbatas. |

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

Menunjukkan cara menyimpan dokumen dalam format Pdf dengan tata letak halaman A4 tanpa batas ketinggian.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// Simpan dokumen.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
```

### Lihat juga

* ruang nama [Aspose.Note.Saving](../../aspose.note.saving/)
* perakitan [Aspose.Note](../../)


