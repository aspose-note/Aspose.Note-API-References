---
title: PdfSaveOptions.PageSettings
second_title: Aspose.Note untuk Referensi .NET API
description: PdfSaveOptions Properti. Mendapat atau mengatur pengaturan halaman untuk setiap halaman dalam dokumen. Secara default tergantung pada CurrentUICulture Budaya AS memiliki pengaturan huruf yang lain memiliki pengaturan A4.
type: docs
weight: 40
url: /id/net/aspose.note.saving/pdfsaveoptions/pagesettings/
---
## PdfSaveOptions.PageSettings property

Mendapat atau mengatur pengaturan halaman untuk setiap halaman dalam dokumen. Secara default tergantung pada CurrentUICulture, *Budaya AS memiliki pengaturan huruf, yang lain memiliki pengaturan A4.

```csharp
public PageSettings PageSettings { get; set; }
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

* class [PageSettings](../../pagesettings/)
* class [PdfSaveOptions](../)
* ruang nama [Aspose.Note.Saving](../../pdfsaveoptions/)
* perakitan [Aspose.Note](../../../)


