---
title: Class TextStyle
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.TextStyle kelas. Menentukan gaya teks.
type: docs
weight: 970
url: /id/net/aspose.note/textstyle/
---
## TextStyle class

Menentukan gaya teks.

```csharp
public sealed class TextStyle : Style
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [TextStyle](textstyle/)() | Konstruktor default. |

## Properti

| Nama | Keterangan |
| --- | --- |
| static [Default](../../aspose.note/textstyle/default/) { get; } | Mendapat gaya dengan budaya "en-US". |
| static [DefaultMsOneNoteTitleDateStyle](../../aspose.note/textstyle/defaultmsonenotetitledatestyle/) { get; } | Mendapat gaya default untuk tanggal judul di MS OneNote. |
| static [DefaultMsOneNoteTitleTextStyle](../../aspose.note/textstyle/defaultmsonenotetitletextstyle/) { get; } | Mendapat gaya default untuk teks judul di MS OneNote. |
| static [DefaultMsOneNoteTitleTimeStyle](../../aspose.note/textstyle/defaultmsonenotetitletimestyle/) { get; } | Mendapat gaya default untuk waktu judul di MS OneNote. |
| [FontColor](../../aspose.note/style/fontcolor/) { get; set; } | Mendapat atau mengatur warna font. |
| [FontName](../../aspose.note/style/fontname/) { get; set; } | Mendapat atau menyetel nama font. |
| [FontSize](../../aspose.note/style/fontsize/) { get; set; } | Mendapat atau mengatur ukuran font. |
| [FontStyle](../../aspose.note/style/fontstyle/) { get; } | Mendapatkan gaya font. |
| [Highlight](../../aspose.note/style/highlight/) { get; set; } | Mendapat atau menyetel warna sorotan. |
| [HyperlinkAddress](../../aspose.note/textstyle/hyperlinkaddress/) { get; set; } | Mendapat atau menetapkan alamat hyperlink. Harus ditetapkan jika nilai dari[`IsHyperlink`](./ishyperlink/) properti benar. |
| [IsBold](../../aspose.note/style/isbold/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah gaya teks dicetak tebal. |
| [IsHidden](../../aspose.note/textstyle/ishidden/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah gaya teks disembunyikan. |
| [IsHyperlink](../../aspose.note/textstyle/ishyperlink/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah gaya teks adalah hyperlink. |
| [IsItalic](../../aspose.note/style/isitalic/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah gaya teks miring. |
| [IsMathFormatting](../../aspose.note/textstyle/ismathformatting/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah gaya teks adalah pemformatan matematika. |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah gaya teks dicoret. |
| [IsSubscript](../../aspose.note/style/issubscript/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah gaya teks adalah subskrip. |
| [IsSuperscript](../../aspose.note/style/issuperscript/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah gaya teks adalah superskrip. |
| [IsUnderline](../../aspose.note/style/isunderline/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah gaya teks digarisbawahi. |
| [Language](../../aspose.note/textstyle/language/) { get; set; } | Mendapat atau menyetel bahasa teks. |

## Metode

| Nama | Keterangan |
| --- | --- |
| override [Equals](../../aspose.note/textstyle/equals/#equals_1)(object) | Menentukan apakah objek yang ditentukan sama dengan objek saat ini. |
| [Equals](../../aspose.note/textstyle/equals/#equals)(TextStyle) | Menentukan apakah objek yang ditentukan sama dengan objek saat ini. |
| override [GetHashCode](../../aspose.note/textstyle/gethashcode/)() | Berfungsi sebagai fungsi hash untuk tipe. |

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

Atur bahasa pemeriksaan untuk teks.

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = ParagraphStyle.Default };
text.Append("United States", new TextStyle() { Language = CultureInfo.GetCultureInfo("en-US") })
    .Append(" Germany", new TextStyle() { Language = CultureInfo.GetCultureInfo("de-DE") })
    .Append(" China", new TextStyle() { Language = CultureInfo.GetCultureInfo("zh-CN") });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetProofingLanguageForText.one"));
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

Menunjukkan cara mengikat hyperlink ke teks.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Tasks();

// Buat objek dari kelas Dokumen
Document doc = new Document();

RichText titleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append("Title!");

Outline outline = new Outline()
                      {
                          MaxWidth = 200,
                          MaxHeight = 200,
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };

TextStyle textStyleRed = new TextStyle
                             {
                                 FontColor = Color.Red,
                                 FontName = "Arial",
                                 FontSize = 10,
                             };

TextStyle textStyleHyperlink = new TextStyle
                                   {
                                       IsHyperlink = true,
                                       HyperlinkAddress = "www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// Tambahkan elemen kerangka
outline.AppendChildLast(outlineElem);

// Inisialisasi objek kelas Judul
Title title = new Title() { TitleText = titleText };

// Inisialisasi objek kelas Halaman
Page page = new Note.Page() { Title = title };

// Tambahkan simpul Outline
page.AppendChildLast(outline);

// Tambahkan simpul Halaman
doc.AppendChildLast(page);

// Simpan dokumen OneNote
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

### Lihat juga

* class [Style](../style/)
* ruang nama [Aspose.Note](../../aspose.note/)
* perakitan [Aspose.Note](../../)


