---
title: Class Notebook
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.Notebook kelas. Merupakan notebook Aspose.Note.
type: docs
weight: 410
url: /id/net/aspose.note/notebook/
---
## Notebook class

Merupakan notebook Aspose.Note.

```csharp
public class Notebook : IEnumerable<INotebookChildNode>, INotebookChildNode
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [Notebook](notebook/#constructor)() | Menginisialisasi instance baru dari`Notebook` kelas. |
| [Notebook](notebook/#constructor_1)(Stream) | Menginisialisasi instance baru dari`Notebook` class. Membuka buku catatan OneNote yang sudah ada dari aliran. |
| [Notebook](notebook/#constructor_3)(string) | Menginisialisasi instance baru dari`Notebook` class. Membuka buku catatan OneNote yang sudah ada dari file. |
| [Notebook](notebook/#constructor_2)(Stream, NotebookLoadOptions) | Menginisialisasi instance baru dari`Notebook` class. Membuka buku catatan OneNote yang sudah ada dari aliran. Memungkinkan untuk menentukan opsi pemuatan tambahan. |
| [Notebook](notebook/#constructor_4)(string, NotebookLoadOptions) | Menginisialisasi instance baru dari`Notebook` class. Membuka buku catatan OneNote yang sudah ada dari sebuah file. Memungkinkan untuk menentukan opsi tambahan seperti strategi pemuatan anak ("malas"/instan). |

## Properti

| Nama | Keterangan |
| --- | --- |
| [Color](../../aspose.note/notebook/color/) { get; set; } | Mendapat atau mengatur warna. |
| [Count](../../aspose.note/notebook/count/) { get; } | Mendapat jumlah elemen yang terkandung dalam`Notebook` . |
| [DisplayName](../../aspose.note/notebook/displayname/) { get; set; } | Mendapat atau menyetel nama tampilan. |
| [FileFormat](../../aspose.note/notebook/fileformat/) { get; } | Mendapatkan format file (OneNote 2010, OneNote Online). |
| [Guid](../../aspose.note/notebook/guid/) { get; } | Mendapat id unik global objek. |
| [IsHistoryEnabled](../../aspose.note/notebook/ishistoryenabled/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah riwayat diaktifkan. |
| [Item](../../aspose.note/notebook/item/) { get; } | Mendapat simpul anak notebook dengan indeks yang diberikan. |

## Metode

| Nama | Keterangan |
| --- | --- |
| [AppendChild](../../aspose.note/notebook/appendchild/)(INotebookChildNode) | Menambahkan simpul ke akhir daftar. |
| [GetChildNodes&lt;T1&gt;](../../aspose.note/notebook/getchildnodes/)() | Dapatkan semua simpul anak berdasarkan jenis simpul. |
| [GetEnumerator](../../aspose.note/notebook/getenumerator/)() | Mengembalikan pencacah yang beralih melalui simpul anak dari`Notebook` . |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument)(Stream) | Menambahkan simpul dokumen anak. Membuka dokumen OneNote yang sudah ada dari aliran. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument_2)(string) | Menambahkan simpul dokumen anak. Membuka dokumen OneNote yang sudah ada dari file. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument_1)(Stream, LoadOptions) | Menambahkan simpul dokumen anak. Membuka dokumen OneNote yang sudah ada dari aliran. Memungkinkan untuk menentukan opsi pemuatan tambahan. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument_3)(string, LoadOptions) | Menambahkan simpul dokumen anak. Membuka dokumen OneNote yang sudah ada dari file. Memungkinkan untuk menentukan opsi pemuatan tambahan. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook)(Stream) | Menambahkan node buku catatan anak. Membuka buku catatan OneNote yang sudah ada dari aliran. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook_2)(string) | Menambahkan simpul buku catatan anak. Membuka buku catatan OneNote yang sudah ada dari file. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook_1)(Stream, NotebookLoadOptions) | Menambahkan node buku catatan anak. Membuka buku catatan OneNote yang sudah ada dari aliran. Memungkinkan untuk menentukan opsi pemuatan tambahan. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook_3)(string, NotebookLoadOptions) | Menambahkan node buku catatan anak. Membuka buku catatan OneNote yang sudah ada dari file. Memungkinkan untuk menentukan opsi pemuatan tambahan. |
| [RemoveChild](../../aspose.note/notebook/removechild/)(INotebookChildNode) | Menghapus simpul anak. |
| [Save](../../aspose.note/notebook/save/#save)(Stream) | Menyimpan dokumen OneNote ke aliran. |
| [Save](../../aspose.note/notebook/save/#save_3)(string) | Menyimpan dokumen OneNote ke file. |
| [Save](../../aspose.note/notebook/save/#save_2)(Stream, NotebookSaveOptions) | Menyimpan dokumen OneNote ke aliran menggunakan opsi penyimpanan yang ditentukan. |
| [Save](../../aspose.note/notebook/save/#save_1)(Stream, SaveFormat) | Menyimpan dokumen OneNote ke aliran dalam format yang ditentukan. |
| [Save](../../aspose.note/notebook/save/#save_5)(string, NotebookSaveOptions) | Menyimpan dokumen OneNote ke file menggunakan opsi penyimpanan yang ditentukan. |
| [Save](../../aspose.note/notebook/save/#save_4)(string, SaveFormat) | Menyimpan dokumen OneNote ke file dalam format yang ditentukan. |

### Contoh

Menunjukkan cara menyimpan buku catatan.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_NoteBook();

var notebook = new Notebook();

dataDir = dataDir + "test_out.onetoc2";

// Simpan Buku Catatan
notebook.Save(dataDir);
```

Menunjukkan cara menyimpan buku catatan dalam format pdf.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Muat Buku Catatan OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Simpan Buku Catatan
notebook.Save(dataDir);
```

Menunjukkan cara menyimpan buku catatan sebagai gambar.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Muat Buku Catatan OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToImage_out.png";

// Simpan Buku Catatan
notebook.Save(dataDir);
```

Menunjukkan cara mendapatkan semua teks dari buku catatan.

```csharp
string inputFile = "notebook.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

Notebook rootNotebook = new Notebook(dataDir + inputFile);

IList<RichText> allRichTextNodes = rootNotebook.GetChildNodes<RichText>();
foreach (RichText richTextNode in allRichTextNodes)
{
    Console.WriteLine(richTextNode.Text);
}
```

Menunjukkan cara menyimpan buku catatan yang diratakan dalam format pdf.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Muat Buku Catatan OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Simpan Buku Catatan
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

Menunjukkan cara mengulangi dokumen buku catatan yang memuatnya dengan malas.

```csharp
string inputFile = "Notizbuch öffnen.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

// Secara default memuat anak-anak adalah "malas".
Notebook notebook = new Notebook(dataDir + inputFile);

foreach (var notebookChildNode in notebook.OfType<Document>()) 
{
    // Pemuatan sebenarnya dari dokumen anak hanya terjadi di sini.
    // Lakukan sesuatu dengan dokumen anak
}
```

Memperlihatkan cara menambahkan bagian baru ke buku catatan.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Muat Buku Catatan OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Tambahkan anak baru ke Notebook
notebook.AppendChild(new Document(dataDir + "Neuer Abschnitt 1.one"));

dataDir = dataDir + "AddChildNode_out.onetoc2";

// Simpan Buku Catatan
notebook.Save(dataDir);
```

Menunjukkan cara memuat notebook dari aliran.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
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

Menunjukkan cara menyimpan buku catatan sebagai gambar dengan opsi yang ditentukan.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Muat Buku Catatan OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// Simpan Buku Catatan
notebook.Save(dataDir, notebookSaveOptions);
```

Menunjukkan cara menyimpan buku catatan yang diratakan sebagai gambar.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Muat Buku Catatan OneNote
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Simpan Buku Catatan
notebook.Save(dataDir, notebookSaveOptions);
```

Memperlihatkan cara menghapus bagian dari buku catatan.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Muat Buku Catatan OneNote
var notebook = new Notebook(dataDir + "test.onetoc2");

// Telusuri node anaknya untuk mencari item anak yang diinginkan
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // Hapus Item Anak dari Notebook
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// Simpan Buku Catatan
notebook.Save(dataDir);
```

Memperlihatkan cara mengulang melalui dokumen buku catatan yang dimuat sebelumnya.

```csharp
// Secara default memuat anak-anak adalah "malas".
// Oleh karena itu untuk pemuatan instan telah dilakukan,
// Anda perlu menyetel bendera NotebookLoadOptions.InstantLoading.
NotebookLoadOptions loadOptions = new NotebookLoadOptions { InstantLoading = true };

String inputFile = "Notizbuch öffnen.onetoc2";
String dataDir = RunExamples.GetDataDir_NoteBook();
Notebook notebook = new Notebook(dataDir + inputFile, loadOptions);

// Semua dokumen anak sudah dimuat.
foreach (INotebookChildNode notebookChildNode in notebook.OfType<Document>()) 
{
   // Lakukan sesuatu dengan dokumen anak
}
```

Memperlihatkan cara melewati konten buku catatan.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = "Open Notebook.onetoc2";
try
{
    var notebook = new Notebook(dataDir + fileName);
    foreach (var notebookChildNode in notebook)
    {
        Console.WriteLine(notebookChildNode.DisplayName);
        if (notebookChildNode is Document)
        {
            // Lakukan sesuatu dengan dokumen anak
        }
        else if (notebookChildNode is Notebook)
        {
            // Lakukan sesuatu dengan buku catatan anak
        }
    }
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
```

### Lihat juga

* interface [INotebookChildNode](../inotebookchildnode/)
* ruang nama [Aspose.Note](../../aspose.note/)
* perakitan [Aspose.Note](../../)


