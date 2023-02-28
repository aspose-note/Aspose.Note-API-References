---
title: Class Title
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.Title kelas. Merupakan judul.
type: docs
weight: 980
url: /id/net/aspose.note/title/
---
## Title class

Merupakan judul.

```csharp
public sealed class Title : CompositeNodeBase, ICompositeNode<RichText>, IPageChildNode
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [Title](title/#constructor)() | Menginisialisasi instance baru dari`Title` kelas. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Mendapat dokumen dari node. |
| [HorizontalOffset](../../aspose.note/title/horizontaloffset/) { get; set; } | Mendapat atau menyetel offset horizontal. |
| override [IsComposite](../../aspose.note/title/iscomposite/) { get; } | Mendapat nilai yang menunjukkan apakah simpul ini komposit. Jika true node dapat memiliki node anak. |
| [LastModifiedTime](../../aspose.note/title/lastmodifiedtime/) { get; set; } | Mendapatkan atau menyetel waktu modifikasi terakhir. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Mendapat node berikutnya pada tingkat pohon node yang sama. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Mendapat tipe node. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Mendapat simpul induk. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Mendapat simpul sebelumnya pada tingkat pohon simpul yang sama. |
| [TitleDate](../../aspose.note/title/titledate/) { get; set; } | Mendapat atau menetapkan representasi string dari tanggal dalam judul. |
| [TitleText](../../aspose.note/title/titletext/) { get; set; } | Mendapat atau menyetel teks judul. |
| [TitleTime](../../aspose.note/title/titletime/) { get; set; } | Mendapat atau menetapkan representasi string waktu dalam judul. |
| [VerticalOffset](../../aspose.note/title/verticaloffset/) { get; set; } | Mendapat atau menyetel offset vertikal. |

## Metode

| Nama | Keterangan |
| --- | --- |
| override [Accept](../../aspose.note/title/accept/)(DocumentVisitor) | Menerima pengunjung node. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/title/getchildnodes/#getchildnodes_1)() | Dapatkan semua simpul anak berdasarkan jenis simpul. |
| [GetEnumerator](../../aspose.note/title/getenumerator/)() | Mengembalikan pencacah yang beralih melalui simpul anak dari`Title` . |

### Contoh

Menunjukkan cara mengedit riwayat halaman.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Pages();

// Muat dokumen OneNote dan dapatkan anak pertama           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.RemoveRange(0, 1);

pageHistory[0] = new Page(document);
if (pageHistory.Count > 1)
{
    pageHistory[1].Title.TitleText.Text = "New Title";

    pageHistory.Add(new Page(document));

    pageHistory.Insert(1, new Page(document));

    document.Save(dataDir + "ModifyPageHistory_out.one");
}
```

Menunjukkan cara mengatur judul untuk halaman.

```csharp
string dataDir = RunExamples.GetDataDir_Text();
string outputPath = dataDir + "CreateTitleMsStyle_out.one";

var doc = new Document();
var page = new Page(doc);

page.Title = new Title(doc)
{
    TitleText = new RichText(doc)
    {
        Text = "Title text.",
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleDate = new RichText(doc)
    {
        Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture),
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleTime = new RichText(doc)
    {
        Text = "12:34",
        ParagraphStyle = ParagraphStyle.Default
    }
};

doc.AppendChildLast(page);

doc.Save(outputPath);
```

Menunjukkan cara membuat dokumen dan menyimpannya dalam format html menggunakan opsi default.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Inisialisasi dokumen OneNote
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

// Gaya default untuk semua teks dalam dokumen.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// Simpan ke dalam format HTML
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

Menunjukkan cara membuat dokumen dan menyimpan dalam format html rentang halaman yang ditentukan.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Inisialisasi dokumen OneNote
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Gaya default untuk semua teks dalam dokumen.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// Simpan ke dalam format HTML
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

Menunjukkan cara membuat dokumen dengan halaman berjudul.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Buat objek dari kelas Dokumen
Document doc = new Aspose.Note.Document();

// Inisialisasi objek kelas Halaman
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Gaya default untuk semua teks dalam dokumen.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Tetapkan properti judul halaman
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Tambahkan simpul Halaman dalam dokumen
doc.AppendChildLast(page);

// Simpan dokumen OneNote
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

Menunjukkan cara menyimpan dokumen dalam berbagai format.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Inisialisasi Dokumen baru
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// Inisialisasi Halaman baru
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Gaya default untuk semua teks dalam dokumen.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Tambahkan simpul halaman
doc.AppendChildLast(page);

// Simpan dokumen OneNote dalam berbagai format, atur ukuran font teks dan deteksi perubahan tata letak secara manual.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

### Lihat juga

* class [CompositeNodeBase](../compositenodebase/)
* interface [ICompositeNode&lt;T&gt;](../icompositenode-1/)
* class [RichText](../richtext/)
* interface [IPageChildNode](../ipagechildnode/)
* ruang nama [Aspose.Note](../../aspose.note/)
* perakitan [Aspose.Note](../../)


