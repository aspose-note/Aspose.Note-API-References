---
title: PageSettings.A4NoHeightLimit
second_title: Aspose.Note untuk Referensi .NET API
description: PageSettings Properti. Mendapat pengaturan untuk halaman format A4 dengan ketinggian tak terbatas.
type: docs
weight: 20
url: /id/net/aspose.note.saving/pagesettings/a4noheightlimit/
---
## PageSettings.A4NoHeightLimit property

Mendapat pengaturan untuk halaman format A4 dengan ketinggian tak terbatas.

```csharp
public static PageSettings A4NoHeightLimit { get; }
```

### Contoh

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

* class [PageSettings](../)
* ruang nama [Aspose.Note.Saving](../../pagesettings/)
* perakitan [Aspose.Note](../../../)


