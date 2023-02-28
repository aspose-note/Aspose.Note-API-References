---
title: Class Image
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.Image kelas. Merupakan Gambar.
type: docs
weight: 250
url: /id/net/aspose.note/image/
---
## Image class

Merupakan Gambar.

```csharp
public sealed class Image : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [Image](image/#constructor)() | Menginisialisasi instance baru dari`Image` kelas. |
| [Image](image/#constructor_4)(string, Stream) | Menginisialisasi instance baru dari`Image` kelas. |
| [Image](image/#constructor_5)(string, string, string) | Menginisialisasi instance baru dari`Image` kelas. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [Alignment](../../aspose.note/image/alignment/) { get; set; } | Mendapat atau menyetel perataan. |
| [AlternativeTextDescription](../../aspose.note/image/alternativetextdescription/) { get; set; } | Mendapat atau menyetel isi teks alternatif untuk gambar. |
| [AlternativeTextTitle](../../aspose.note/image/alternativetexttitle/) { get; set; } | Mendapat atau menetapkan judul teks alternatif untuk gambar. |
| [Bytes](../../aspose.note/image/bytes/) { get; } | Mendapatkan penyimpanan data gambar. |
| [Document](../../aspose.note/node/document/) { get; } | Mendapat dokumen dari node. |
| [FileName](../../aspose.note/image/filename/) { get; } | Mendapatkan nama file. |
| [FilePath](../../aspose.note/image/filepath/) { get; } | Mendapat jalur ke file gambar. |
| [Format](../../aspose.note/image/format/) { get; } | Mendapatkan format gambar. |
| [Height](../../aspose.note/image/height/) { get; set; } | Mendapat atau mengatur ketinggian. Ini adalah tinggi sebenarnya dari gambar di dokumen MS OneNote. |
| [HorizontalOffset](../../aspose.note/image/horizontaloffset/) { get; set; } | Mendapat atau menyetel offset horizontal. |
| [HyperlinkUrl](../../aspose.note/image/hyperlinkurl/) { get; set; } | Mendapatkan atau menyetel hyperlink yang terkait dengan gambar. |
| [IsBackground](../../aspose.note/image/isbackground/) { get; set; } | Mendapat apakah gambar adalah gambar latar belakang. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | Mendapat nilai yang menunjukkan apakah simpul ini komposit. Jika true node dapat memiliki node anak. |
| [LastModifiedTime](../../aspose.note/image/lastmodifiedtime/) { get; set; } | Mendapatkan atau menetapkan waktu modifikasi terakhir. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Mendapat node berikutnya pada tingkat pohon node yang sama. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Mendapat tipe node. |
| [OriginalHeight](../../aspose.note/image/originalheight/) { get; } | Mendapat tinggi aslinya. Ini adalah lebar asli gambar, sebelum diubah ukurannya. |
| [OriginalWidth](../../aspose.note/image/originalwidth/) { get; } | Mendapatkan lebar aslinya. Ini adalah lebar asli gambar, sebelum diubah ukurannya. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Mendapat simpul induk. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Mendapat simpul sebelumnya pada tingkat pohon simpul yang sama. |
| [Tags](../../aspose.note/image/tags/) { get; } | Mendapat daftar semua tag paragraf. |
| [VerticalOffset](../../aspose.note/image/verticaloffset/) { get; set; } | Mendapat atau menyetel offset vertikal. |
| [Width](../../aspose.note/image/width/) { get; set; } | Mendapat atau mengatur lebar. Ini adalah lebar sebenarnya dari gambar di dokumen MS OneNote. |

## Metode

| Nama | Keterangan |
| --- | --- |
| override [Accept](../../aspose.note/image/accept/)(DocumentVisitor) | Menerima pengunjung node. |

### Contoh

Menunjukkan cara mengikat hyperlink ke gambar.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://gambar.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

Menunjukkan cara menyetel deskripsi teks untuk gambar.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Images();

var document = new Document();
var page = new Page(document);
var image = new Image(document, dataDir + "image.jpg")
            {
                AlternativeTextTitle = "This is an image's title!",
                AlternativeTextDescription = "And this is an image's description!"
            };
page.AppendChildLast(image);
document.AppendChildLast(page);

dataDir = dataDir + "ImageAlternativeText_out.one";
document.Save(dataDir);
```

Menunjukkan cara mendapatkan gambar dari dokumen.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Images();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Dapatkan semua node Gambar
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Simpan byte gambar ke file
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

Menunjukkan cara mendapatkan informasi meta gambar.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Images();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Dapatkan semua node Gambar
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

Menunjukkan cara menambahkan gambar baru dengan tag.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Tags();

// Buat objek dari kelas Dokumen
Document doc = new Document();

// Inisialisasi objek kelas Halaman
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inisialisasi objek kelas Outline
Outline outline = new Outline(doc);

// Menginisialisasi objek kelas OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Memuat gambar
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

// Sisipkan gambar di simpul dokumen
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// Tambahkan simpul elemen kerangka
outline.AppendChildLast(outlineElem);

// Tambahkan simpul kerangka
page.AppendChildLast(outline);

// Tambahkan simpul halaman
doc.AppendChildLast(page);

// Simpan dokumen OneNote
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
```

Menunjukkan cara menambahkan gambar dari file ke dokumen dengan properti yang ditentukan pengguna.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Images();

// Muat dokumen dari aliran.
Document doc = new Document(dataDir + "Aspose.one");

// Dapatkan halaman pertama dokumen.
Aspose.Note.Page page = doc.FirstChild;

// Memuat gambar dari file.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Ubah ukuran gambar sesuai kebutuhan Anda (opsional).
                              Width = 100,
                              Height = 100,

                              // Tetapkan lokasi gambar di halaman (opsional).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // Atur perataan gambar
                              Alignment = HorizontalAlignment.Right
                          };

// Tambahkan gambar ke halaman.
page.AppendChildLast(image);
```

Menunjukkan cara menambahkan gambar dari aliran ke dokumen.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Images();

// Buat objek dari kelas Dokumen
Document doc = new Document();

// Inisialisasi objek kelas Halaman
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // Muat gambar kedua menggunakan nama gambar, ekstensi, dan aliran.
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // Atur perataan gambar
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// Simpan dokumen OneNote
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

Menunjukkan cara menambahkan gambar dari file ke dokumen.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Images();

// Buat objek dari kelas Dokumen
Document doc = new Document();

// Inisialisasi objek kelas Halaman
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inisialisasi objek kelas Outline dan atur properti offset
Outline outline = new Outline(doc);

// Menginisialisasi objek kelas OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Muat gambar dengan jalur file.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Atur perataan gambar
                              Alignment = HorizontalAlignment.Right
                          };

// Menambahkan gambar
outlineElem.AppendChildLast(image);

// Tambahkan elemen kerangka
outline.AppendChildLast(outlineElem);

// Tambahkan simpul Outline
page.AppendChildLast(outline);

// Tambahkan simpul Halaman
doc.AppendChildLast(page);

// Simpan dokumen OneNote
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

### Lihat juga

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [IPageChildNode](../ipagechildnode/)
* interface [ITaggable](../itaggable/)
* ruang nama [Aspose.Note](../../aspose.note/)
* perakitan [Aspose.Note](../../)


