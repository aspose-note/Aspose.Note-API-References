---
title: Class NumberList
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.NumberList kelas. Mewakili daftar bernomor atau berpoin.
type: docs
weight: 440
url: /id/net/aspose.note/numberlist/
---
## NumberList class

Mewakili daftar bernomor atau berpoin.

```csharp
public class NumberList
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [NumberList](numberlist/#constructor_1)(string, string, int) | Menginisialisasi instance baru dari`NumberList`class. Instance ini mewakili daftar berpoin. |
| [NumberList](numberlist/#constructor)(string, NumberFormat, string, int) | Menginisialisasi instance baru dari`NumberList` class. Contoh ini mewakili daftar bernomor. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [Font](../../aspose.note/numberlist/font/) { get; set; } | Mendapat atau menetapkan nama font. |
| [FontColor](../../aspose.note/numberlist/fontcolor/) { get; set; } | Mendapat atau mengatur warna font. |
| [FontSize](../../aspose.note/numberlist/fontsize/) { get; set; } | Mendapat atau mengatur ukuran font. |
| [Format](../../aspose.note/numberlist/format/) { get; set; } | Mendapat atau mengatur format header baris. Untuk daftar berpoin mewakili simbol poin. |
| [IsBold](../../aspose.note/numberlist/isbold/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah gaya teks dicetak tebal. |
| [IsItalic](../../aspose.note/numberlist/isitalic/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah gaya teks miring. |
| [LastModifiedTime](../../aspose.note/numberlist/lastmodifiedtime/) { get; set; } | Mendapatkan atau menyetel waktu modifikasi terakhir. |
| [NumberFormat](../../aspose.note/numberlist/numberformat/) { get; set; } | Mendapat atau mengatur format angka yang digunakan untuk grup objek yang diberi nomor secara otomatis. Harus nol untuk daftar berpoin. |
| [Restart](../../aspose.note/numberlist/restart/) { get; set; } | Mendapat atau menyetel nilai numerik yang menggantikan nilai angka otomatis dari item daftar. |

## Metode

| Nama | Keterangan |
| --- | --- |
| [Equals](../../aspose.note/numberlist/equals/#equals)(NumberList) | Menentukan apakah objek yang ditentukan sama dengan objek saat ini. |
| override [Equals](../../aspose.note/numberlist/equals/#equals_1)(object) | Menentukan apakah objek yang ditentukan sama dengan objek saat ini. |
| override [GetHashCode](../../aspose.note/numberlist/gethashcode/)() | Berfungsi sebagai fungsi hash untuk tipe. |
| [GetNumberedListHeader](../../aspose.note/numberlist/getnumberedlistheader/)(int) | Mendapat header daftar bernomor. |

### Contoh

Memperlihatkan cara mengambil informasi tentang pemformatan daftar.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// Ambil kumpulan simpul dari elemen kerangka
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// Iterasi melalui setiap node
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // Ambil nama font
        Console.WriteLine("Font Name: " + list.Font);

        // Ambil panjang font
        Console.WriteLine("Font Length: " + list.Font.Length);

        // Ambil ukuran font
        Console.WriteLine("Font Size: " + list.FontSize);

        // Ambil warna font
        Console.WriteLine("Font Color: " + list.FontColor);

        // Ambil format
        Console.WriteLine("Font format: " + list.Format);

        // Centang tebal
        Console.WriteLine("Is bold: " + list.IsBold);

        // Centang miring
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

Menunjukkan cara menyisipkan daftar baru dengan penomoran Cina.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Inisialisasi dokumen OneNote
Aspose.Note.Document doc = new Aspose.Note.Document();

// Inisialisasi halaman OneNote
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// Terapkan pengaturan gaya teks
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Angka dalam kerangka yang sama secara otomatis bertambah.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

//------------------------
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

//------------------------
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

//------------------------
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// Simpan dokumen OneNote
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

Menunjukkan cara menyisipkan daftar baru dengan penomoran.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Buat objek dari kelas Dokumen
Document doc = new Document();

// Inisialisasi objek kelas Halaman
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inisialisasi objek kelas Outline
Outline outline = new Outline(doc);

// Inisialisasi objek kelas TextStyle dan atur properti pemformatan
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Menginisialisasi objek kelas OutlineElement dan menerapkan penomoran
// Angka dalam kerangka yang sama secara otomatis bertambah.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Tambahkan elemen kerangka
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Tambahkan simpul Outline
page.AppendChildLast(outline);

// Tambahkan simpul Halaman
doc.AppendChildLast(page);

// Simpan dokumen OneNote
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

### Lihat juga

* ruang nama [Aspose.Note](../../aspose.note/)
* perakitan [Aspose.Note](../../)


