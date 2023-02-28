---
title: Class OneSaveOptions
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.Saving.OneSaveOptions kelas. Memungkinkan untuk menentukan opsi tambahan saat menyimpan dokumen ke format OneNote.
type: docs
weight: 810
url: /id/net/aspose.note.saving/onesaveoptions/
---
## OneSaveOptions class

Memungkinkan untuk menentukan opsi tambahan saat menyimpan dokumen ke format OneNote.

```csharp
public sealed class OneSaveOptions : SaveOptions
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [OneSaveOptions](onesaveoptions/)() | Konstruktor default. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [DocumentPassword](../../aspose.note.saving/onesaveoptions/documentpassword/) { get; set; } | Mendapatkan atau menyetel kata sandi untuk mengenkripsi konten dokumen. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | Mendapatkan atau menyetel pengaturan font untuk digunakan saat menyimpan |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | Mendapat atau mengatur jumlah halaman yang akan disimpan. Secara default adalahMaxValue yang berarti semua halaman dokumen akan dirender. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | Mendapat atau menetapkan indeks halaman pertama yang akan disimpan. Secara default adalah 0. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | Mendapatkan format penyimpanan dokumen. |

### Contoh

Menunjukkan cara menyimpan dokumen dengan enkripsi.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

Menunjukkan cara menyimpan dokumen menggunakan OneSaveOptions.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

### Lihat juga

* class [SaveOptions](../saveoptions/)
* ruang nama [Aspose.Note.Saving](../../aspose.note.saving/)
* perakitan [Aspose.Note](../../)


