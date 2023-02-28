---
title: Class LoadOptions
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.LoadOptions kelas. Opsi yang digunakan untuk memuat dokumen.
type: docs
weight: 320
url: /id/net/aspose.note/loadoptions/
---
## LoadOptions class

Opsi yang digunakan untuk memuat dokumen.

```csharp
public class LoadOptions
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [LoadOptions](loadoptions/)() | Konstruktor default. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [DocumentPassword](../../aspose.note/loadoptions/documentpassword/) { get; set; } | Mendapat atau menyetel kata sandi untuk konten dokumen terenkripsi. Nilai diabaikan jika dokumen tidak dilindungi kata sandi. |
| [LoadHistory](../../aspose.note/loadoptions/loadhistory/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah pemuat dokumen harus mengabaikan riwayat. Gunakan opsi ini untuk mengurangi penggunaan memori dan CPU. Nilai defaultnya adalah`BENAR` . |

### Contoh

Menunjukkan bagaimana sebuah dokumen terenkripsi.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

Menunjukkan cara membuat buku catatan terenkripsi.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
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

* ruang nama [Aspose.Note](../../aspose.note/)
* perakitan [Aspose.Note](../../)


