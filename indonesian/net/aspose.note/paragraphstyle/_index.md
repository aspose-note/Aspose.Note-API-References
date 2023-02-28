---
title: Class ParagraphStyle
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.ParagraphStyle kelas. Pengaturan gaya teks yang akan digunakan jika tidak ada objek TextStyle yang cocokStyles koleksi baik objek ini tidak menentukan pengaturan yang diperlukan.
type: docs
weight: 510
url: /id/net/aspose.note/paragraphstyle/
---
## ParagraphStyle class

Pengaturan gaya teks yang akan digunakan jika tidak ada objek TextStyle yang cocokStyles koleksi baik objek ini tidak menentukan pengaturan yang diperlukan.

```csharp
public sealed class ParagraphStyle : Style, IEquatable<ParagraphStyle>
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [ParagraphStyle](paragraphstyle/)() | Menginisialisasi instance baru dari`ParagraphStyle` kelas. |

## Properti

| Nama | Keterangan |
| --- | --- |
| static [Default](../../aspose.note/paragraphstyle/default/) { get; } | Mendapatkan ParagraphStyle dengan pengaturan default. |
| [FontColor](../../aspose.note/style/fontcolor/) { get; set; } | Mendapat atau mengatur warna font. |
| [FontName](../../aspose.note/style/fontname/) { get; set; } | Mendapat atau menyetel nama font. |
| [FontSize](../../aspose.note/style/fontsize/) { get; set; } | Mendapat atau mengatur ukuran font. |
| [FontStyle](../../aspose.note/style/fontstyle/) { get; } | Mendapatkan gaya font. |
| [Highlight](../../aspose.note/style/highlight/) { get; set; } | Mendapat atau menyetel warna sorotan. |
| [IsBold](../../aspose.note/style/isbold/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah gaya teks dicetak tebal. |
| [IsItalic](../../aspose.note/style/isitalic/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah gaya teks miring. |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah gaya teks dicoret. |
| [IsSubscript](../../aspose.note/style/issubscript/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah gaya teks adalah subskrip. |
| [IsSuperscript](../../aspose.note/style/issuperscript/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah gaya teks adalah superskrip. |
| [IsUnderline](../../aspose.note/style/isunderline/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah gaya teks digarisbawahi. |

## Metode

| Nama | Keterangan |
| --- | --- |
| override [Equals](../../aspose.note/paragraphstyle/equals/#equals_1)(object) | Menentukan apakah objek yang ditentukan sama dengan objek saat ini. |
| [Equals](../../aspose.note/paragraphstyle/equals/#equals)(ParagraphStyle) | Menentukan apakah objek yang ditentukan sama dengan objek saat ini. |
| override [GetHashCode](../../aspose.note/paragraphstyle/gethashcode/)() | Berfungsi sebagai fungsi hash untuk tipe. |

### Contoh

Mari kita tekankan judul halaman di antara header lainnya dengan memperbesar ukuran font.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Muat dokumen ke Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Ulangi judul halaman.
foreach (var title in document.Select(e => e.Title.TitleText))
{
    title.ParagraphStyle.FontSize = 24;
    title.ParagraphStyle.IsBold = true;

    foreach (var run in title.TextRuns)
    {
        run.Style.FontSize = 24;
        run.Style.IsBold = true;
    }
}

document.Save(Path.Combine(dataDir, "ChangePageTitleStyle.pdf"));
```

Mari kita tekankan perubahan teks terbaru dengan menyorot.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Muat dokumen ke Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Ubah node RichText minggu lalu.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // Tetapkan warna sorotan
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // Tetapkan warna sorotan
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

Memanipulasi menurut format teks menggunakan gaya paragraf.

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = new ParagraphStyle() { FontName = "Courier New", FontSize = 20 } }
                .Append($"DefaultParagraphFontAndSize{Environment.NewLine}")
                .Append($"OnlyDefaultParagraphFont{Environment.NewLine}", new TextStyle() { FontSize = 14 })
                .Append("OnlyDefaultParagraphFontSize", new TextStyle() { FontName = "Verdana" });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetDefaultParagraphStyle.one"));
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

Menunjukkan cara menyisipkan lis berpoin baru.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Buat objek dari kelas Dokumen
Aspose.Note.Document doc = new Aspose.Note.Document();

// Inisialisasi objek kelas Halaman
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inisialisasi objek kelas Outline
Outline outline = new Outline(doc);

// Inisialisasi objek kelas TextStyle dan atur properti pemformatan
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Menginisialisasi objek kelas OutlineElement dan menerapkan peluru
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// Inisialisasi objek kelas RichText dan terapkan gaya teks
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
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
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
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

* class [Style](../style/)
* ruang nama [Aspose.Note](../../aspose.note/)
* perakitan [Aspose.Note](../../)


