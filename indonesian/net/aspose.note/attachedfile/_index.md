---
title: Class AttachedFile
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.AttachedFile kelas. Merupakan lampiran file.
type: docs
weight: 10
url: /id/net/aspose.note/attachedfile/
---
## AttachedFile class

Merupakan lampiran file.

```csharp
public class AttachedFile : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [AttachedFile](attachedfile/#constructor)() | Menginisialisasi instance baru dari`AttachedFile` kelas. |
| [AttachedFile](attachedfile/#constructor_6)(string, Stream) | Menginisialisasi instance baru dari`AttachedFile` kelas. |
| [AttachedFile](attachedfile/#constructor_7)(string, Stream, ImageFormat) | Menginisialisasi instance baru dari`AttachedFile` kelas. |
| [AttachedFile](attachedfile/#constructor_8)(string, Stream, Stream, ImageFormat) | Menginisialisasi instance baru dari`AttachedFile` kelas. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [Alignment](../../aspose.note/attachedfile/alignment/) { get; set; } | Mendapat atau menyetel perataan. |
| [AlternativeTextDescription](../../aspose.note/attachedfile/alternativetextdescription/) { get; set; } | Mendapat atau menyetel isi teks alternatif untuk ikon file terlampir. |
| [AlternativeTextTitle](../../aspose.note/attachedfile/alternativetexttitle/) { get; set; } | Mendapat atau menetapkan judul teks alternatif untuk ikon file terlampir. |
| [Bytes](../../aspose.note/attachedfile/bytes/) { get; } | Mendapatkan data biner untuk file yang disematkan. |
| [Document](../../aspose.note/node/document/) { get; } | Mendapat dokumen dari node. |
| [Extension](../../aspose.note/attachedfile/extension/) { get; } | Mendapat ekstensi file tersemat. |
| [FileName](../../aspose.note/attachedfile/filename/) { get; } | Mendapat nama file tersemat. |
| [FilePath](../../aspose.note/attachedfile/filepath/) { get; } | Mendapat jalur ke file asli. |
| [Height](../../aspose.note/attachedfile/height/) { get; } | Mendapat tinggi asli dari ikon file tersemat. |
| [HorizontalOffset](../../aspose.note/attachedfile/horizontaloffset/) { get; set; } | Mendapat atau menyetel offset horizontal. |
| [Icon](../../aspose.note/attachedfile/icon/) { get; } | Mendapatkan data biner untuk ikon yang diasosiasikan dengan file tersemat. |
| [IconExtension](../../aspose.note/attachedfile/iconextension/) { get; } | Mendapatkan ekstensi ikon. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | Mendapat nilai yang menunjukkan apakah simpul ini komposit. Jika true node dapat memiliki node anak. |
| [IsPrintout](../../aspose.note/attachedfile/isprintout/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah tampilan file adalah cetakan. |
| [IsSizeSetByUser](../../aspose.note/attachedfile/issizesetbyuser/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah nilai ukuran ikon diperbarui secara eksplisit oleh pengguna. |
| [LastModifiedTime](../../aspose.note/attachedfile/lastmodifiedtime/) { get; set; } | Mendapatkan atau menyetel waktu modifikasi terakhir. |
| [MaxHeight](../../aspose.note/attachedfile/maxheight/) { get; set; } | Mendapatkan atau menyetel tinggi maksimum untuk menampilkan ikon file tersemat. |
| [MaxWidth](../../aspose.note/attachedfile/maxwidth/) { get; set; } | Mendapat atau menyetel lebar maksimum untuk menampilkan ikon file tersemat. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Mendapat node berikutnya pada tingkat pohon node yang sama. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Mendapat tipe node. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Mendapat simpul induk. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Mendapat simpul sebelumnya pada tingkat pohon simpul yang sama. |
| [Tags](../../aspose.note/attachedfile/tags/) { get; } | Mendapat daftar semua tag paragraf. |
| [Text](../../aspose.note/attachedfile/text/) { get; set; } | Mendapat atau mengatur representasi teks dari file yang disematkan. String TIDAK BOLEH mengandung karakter apa pun dari nilai 10 (line feed) atau 13 (carriage return). |
| [VerticalOffset](../../aspose.note/attachedfile/verticaloffset/) { get; set; } | Mendapat atau menyetel offset vertikal. |
| [Width](../../aspose.note/attachedfile/width/) { get; } | Mendapatkan lebar asli dari ikon file tersemat. |

## Metode

| Nama | Keterangan |
| --- | --- |
| override [Accept](../../aspose.note/attachedfile/accept/)(DocumentVisitor) | Menerima pengunjung node. |

### Contoh

Menunjukkan cara mendapatkan konten dari file terlampir.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Attachments();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "Sample1.one");

// Dapatkan daftar node file terlampir
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// Iterasi melalui semua node
foreach (AttachedFile file in nodes)
{
    // Memuat file terlampir ke objek aliran
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // Buat file lokal
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // Salin aliran file
            CopyStream(outputStream, fileStream);
        }
    }
}
```

Memperlihatkan cara menambahkan file ke dokumen menggunakan jalur file.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Attachments();

// Buat objek dari kelas Dokumen
Document doc = new Document();

// Inisialisasi objek kelas Halaman
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inisialisasi objek kelas Outline
Outline outline = new Outline(doc);

// Menginisialisasi objek kelas OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Menginisialisasi objek kelas AttachedFile
AttachedFile attachedFile = new AttachedFile(doc,  dataDir + "attachment.txt");

// Tambahkan file terlampir
outlineElem.AppendChildLast(attachedFile);

// Tambahkan simpul elemen kerangka
outline.AppendChildLast(outlineElem);

// Tambahkan simpul kerangka
page.AppendChildLast(outline);

// Tambahkan simpul halaman
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileByPath_out.one";
doc.Save(dataDir);
```

Menunjukkan cara menambahkan file dari aliran ke dokumen.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Attachments();

// Buat objek dari kelas Dokumen
Document doc = new Document();

// Inisialisasi objek kelas Halaman
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inisialisasi objek kelas Outline
Outline outline = new Outline(doc);

// Menginisialisasi objek kelas OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // Menginisialisasi objek kelas AttachedFile dan juga meneruskan jalur ikonnya
    AttachedFile attachedFile = new AttachedFile(doc, dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // Tambahkan file terlampir
    outlineElem.AppendChildLast(attachedFile);
}

// Tambahkan simpul elemen kerangka
outline.AppendChildLast(outlineElem);

// Tambahkan simpul kerangka
page.AppendChildLast(outline);

// Tambahkan simpul halaman
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileAndSetIcon_out.one";
doc.Save(dataDir);
```

### Lihat juga

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [IPageChildNode](../ipagechildnode/)
* interface [ITaggable](../itaggable/)
* ruang nama [Aspose.Note](../../aspose.note/)
* perakitan [Aspose.Note](../../)


