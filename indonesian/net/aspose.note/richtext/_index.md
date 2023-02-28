---
title: Class RichText
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.RichText kelas. Merupakan teks kaya.
type: docs
weight: 530
url: /id/net/aspose.note/richtext/
---
## RichText class

Merupakan teks kaya.

```csharp
public sealed class RichText : Node, IEnumerable<char>, IOutlineElementChildNode, ITaggable
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [RichText](richtext/#constructor)() | Menginisialisasi instance baru dari`RichText` kelas. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [Alignment](../../aspose.note/richtext/alignment/) { get; set; } | Mendapat atau menyetel perataan. |
| [Document](../../aspose.note/node/document/) { get; } | Mendapat dokumen dari node. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | Mendapat nilai yang menunjukkan apakah simpul ini komposit. Jika true node dapat memiliki node anak. |
| [LastModifiedTime](../../aspose.note/richtext/lastmodifiedtime/) { get; set; } | Mendapatkan atau menyetel waktu modifikasi terakhir. |
| [Length](../../aspose.note/richtext/length/) { get; } | Mendapatkan panjang teks. |
| [LineSpacing](../../aspose.note/richtext/linespacing/) { get; set; } | Mendapat atau mengatur spasi baris. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Mendapat node berikutnya pada tingkat pohon node yang sama. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Mendapat tipe node. |
| [ParagraphStyle](../../aspose.note/richtext/paragraphstyle/) { get; set; } | Mendapat atau menyetel gaya paragraf. Setelan ini digunakan jika tidak ada objek TextStyle yang cocok diStyles koleksi baik objek ini tidak menentukan pengaturan yang diperlukan. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Mendapat simpul induk. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Mendapat simpul sebelumnya pada tingkat pohon simpul yang sama. |
| [SpaceAfter](../../aspose.note/richtext/spaceafter/) { get; set; } | Mendapat atau menyetel jumlah minimum ruang setelah. |
| [SpaceBefore](../../aspose.note/richtext/spacebefore/) { get; set; } | Mendapat atau menetapkan jumlah ruang minimum sebelumnya. |
| [Tags](../../aspose.note/richtext/tags/) { get; } | Mendapat daftar semua tag paragraf. |
| [Text](../../aspose.note/richtext/text/) { get; set; } | Mendapat atau menyetel teks. String TIDAK BOLEH mengandung karakter apa pun dari nilai 10 (umpan baris). |
| [TextRuns](../../aspose.note/richtext/textruns/) { get; } | Mendapat kumpulan teks berjalan. |

## Metode

| Nama | Keterangan |
| --- | --- |
| override [Accept](../../aspose.note/richtext/accept/)(DocumentVisitor) | Menerima pengunjung node. |
| [Append](../../aspose.note/richtext/append/#append)(string) | Menambahkan string ke rentang teks terakhir. |
| [Append](../../aspose.note/richtext/append/#append_1)(string, TextStyle) | Menambahkan string ke akhir. |
| [AppendFront](../../aspose.note/richtext/appendfront/#appendfront)(string) | Menambahkan string ke depan rentang teks pertama. |
| [AppendFront](../../aspose.note/richtext/appendfront/#appendfront_1)(string, TextStyle) | Menambahkan string ke depan. |
| [Clear](../../aspose.note/richtext/clear/)() | Menghapus konten instance ini. |
| [GetEnumerator](../../aspose.note/richtext/getenumerator/)() | Mengembalikan pencacah yang mengulang melalui karakter objek RichText ini. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof)(char) | Mengembalikan indeks berbasis nol dari kemunculan pertama karakter Unicode yang ditentukan dalam string ini. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_3)(string) | Mengembalikan indeks berbasis nol dari kejadian pertama dari string yang ditentukan dalam contoh ini. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_1)(char, int) | Mengembalikan indeks berbasis nol dari kemunculan pertama karakter Unicode yang ditentukan dalam string ini. Pencarian dimulai pada posisi karakter tertentu. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_4)(string, int) | Mengembalikan indeks berbasis nol dari kemunculan pertama string yang ditentukan dalam contoh ini. Pencarian dimulai pada posisi karakter tertentu. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_8)(string, StringComparison) | Mengembalikan indeks berbasis nol dari kemunculan pertama string yang ditentukan dalam instance saat ini. Parameter menentukan jenis pencarian yang akan digunakan untuk string yang ditentukan. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_2)(char, int, int) | Mengembalikan indeks berbasis nol dari kemunculan pertama karakter tertentu dalam contoh ini. Pencarian dimulai pada posisi karakter tertentu dan memeriksa sejumlah posisi karakter tertentu. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_5)(string, int, int) | Mengembalikan indeks berbasis nol dari kemunculan pertama string yang ditentukan dalam contoh ini. Pencarian dimulai pada posisi karakter tertentu dan memeriksa sejumlah posisi karakter tertentu. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_7)(string, int, StringComparison) | Mengembalikan indeks berbasis nol dari kemunculan pertama string yang ditentukan dalam instance saat ini. Parameter menentukan posisi pencarian awal dalam string saat ini dan jenis pencarian yang akan digunakan untuk string yang ditentukan. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_6)(string, int, int, StringComparison) | Mengembalikan indeks berbasis nol dari kemunculan pertama string yang ditentukan dalam instance saat ini. |
| [Insert](../../aspose.note/richtext/insert/#insert)(int, string) | Menyisipkan string tertentu pada posisi indeks tertentu dalam contoh ini. |
| [Insert](../../aspose.note/richtext/insert/#insert_1)(int, string, TextStyle) | Menyisipkan string tertentu dengan gaya tertentu pada posisi indeks tertentu dalam contoh ini. |
| [Remove](../../aspose.note/richtext/remove/#remove)(int) | Menghapus semua karakter dalam instance saat ini, mulai dari posisi tertentu dan berlanjut hingga posisi terakhir. |
| [Remove](../../aspose.note/richtext/remove/#remove_1)(int, int) | Menghapus jumlah karakter tertentu dalam instance saat ini yang dimulai pada posisi tertentu. |
| [Replace](../../aspose.note/richtext/replace/#replace)(char, char) | Menggantikan semua kemunculan karakter Unicode tertentu dalam contoh ini dengan karakter Unicode lain yang ditentukan. |
| [Replace](../../aspose.note/richtext/replace/#replace_1)(string, string) | Menggantikan semua kemunculan string tertentu dalam contoh saat ini dengan string lain yang ditentukan. |
| [Replace](../../aspose.note/richtext/replace/#replace_2)(string, string, TextStyle) | Menggantikan semua kemunculan string yang ditentukan dalam contoh saat ini dengan string lain yang ditentukan dalam gaya yang ditentukan. |
| [Trim](../../aspose.note/richtext/trim/#trim)() | Menghapus semua karakter spasi putih awal dan akhir. |
| [Trim](../../aspose.note/richtext/trim/#trim_1)(char) | Menghapus semua awalan dan akhiran karakter. |
| [Trim](../../aspose.note/richtext/trim/#trim_2)(params char[]) | Menghapus semua kemunculan awal dan akhir dari serangkaian karakter yang ditentukan dalam larik. |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend)() | Menghapus semua karakter spasi putih yang tertinggal. |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend_1)(char) | Menghapus semua kemunculan karakter. |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend_2)(params char[]) | Menghapus semua kejadian akhir dari sekumpulan karakter yang ditentukan dalam array. |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart)() | Menghapus semua karakter spasi putih di depan. |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart_1)(char) | Menghapus semua kemunculan awal dari karakter tertentu. |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart_2)(params char[]) | Menghapus semua kemunculan awal dari serangkaian karakter yang ditentukan dalam larik. |

### Contoh

Menunjukkan cara mendapatkan semua teks dari dokumen.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Text();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Mengambil teks
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// Cetak teks pada layar keluaran
Console.WriteLine(text);
```

Menunjukkan cara mendapatkan semua teks dari halaman.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Text();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Dapatkan daftar node halaman
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // Mengambil teks
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // Cetak teks pada layar keluaran
    Console.WriteLine(text);
}
```

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

Menunjukkan cara mendapatkan teks dari setiap baris tabel.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Tables();

// Muat dokumen ke Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Dapatkan daftar node tabel
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // Iterasi melalui baris tabel
    foreach (TableRow row in table)
    {
        // Mengambil teks
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // Cetak teks pada layar keluaran
        Console.WriteLine(text);
    }
}
```

Menunjukkan cara mendapatkan teks dari tabel.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Tables();

// Muat dokumen ke Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Dapatkan daftar node tabel
IList<Table> nodes = document.GetChildNodes<Table>();

// Tetapkan jumlah tabel
int tblCount = 0;

foreach (Table table in nodes)
{
    tblCount++;
    Console.WriteLine("table # " + tblCount);

    // Mengambil teks
    string text = string.Join(Environment.NewLine, table.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

    // Cetak teks pada layar keluaran
    Console.WriteLine(text);
}
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

Menunjukkan cara melewati semua halaman dan membuat penggantian dalam teks.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Dapatkan semua node RichText
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Ganti teks bentuk
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

// Simpan ke format file apa pun yang didukung
oneFile.Save(dataDir, SaveFormat.Pdf);
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

Menunjukkan cara mendapatkan teks dari sel tabel.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Tables();

// Muat dokumen ke Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Dapatkan daftar node tabel
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // Iterasi melalui baris tabel
    foreach (TableRow row in table)
    {
        // Dapatkan daftar node TableCell
        // Iterasi melalui sel tabel
        foreach (TableCell cell in row)
        {
            // Mengambil teks
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // Cetak teks pada layar keluaran
            Console.WriteLine(text);
        }
    }
}
```

Menunjukkan cara melewati teks halaman dan membuat pengganti.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// Dapatkan semua node RichText
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Ganti teks bentuk
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// Simpan ke format file apa pun yang didukung
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
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

Menunjukkan cara menambahkan paragraf baru dengan tag.

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
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
RichText text = new RichText(doc) { Text = "OneNote text.", ParagraphStyle = textStyle };
text.Tags.Add(NoteTag.CreateYellowStar());

// Tambahkan simpul teks
outlineElem.AppendChildLast(text);

// Tambahkan simpul elemen kerangka
outline.AppendChildLast(outlineElem);

// Tambahkan simpul kerangka
page.AppendChildLast(outline);

// Tambahkan simpul halaman
doc.AppendChildLast(page);

// Simpan dokumen OneNote
dataDir = dataDir + "AddTextNodeWithTag_out.one";
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

Menunjukkan cara mengakses detail tag.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Tags();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "TagFile.one");

// Dapatkan semua node RichText
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Iterasi melalui setiap node
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // Ambil properti
            Console.WriteLine($"    Completed Time: {noteTag.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTag.CreationTime}");
            Console.WriteLine($"    Font Color: {noteTag.FontColor}");
            Console.WriteLine($"    Status: {noteTag.Status}");
            Console.WriteLine($"    Label: {noteTag.Label}");
            Console.WriteLine($"    Icon: {noteTag.Icon}");
            Console.WriteLine($"    High Light: {noteTag.Highlight}");
        }
    }
}
```

Menunjukkan cara membuat dokumen dengan teks.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Buat objek dari kelas Dokumen
Document doc = new Document();

// Inisialisasi objek kelas Halaman
Page page = new Page(doc);

// Inisialisasi objek kelas Outline
Outline outline = new Outline(doc);

// Menginisialisasi objek kelas OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Inisialisasi objek kelas TextStyle dan atur properti pemformatan
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Inisialisasi objek kelas RichText dan terapkan gaya teks
RichText text = new RichText(doc) { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// Tambahkan simpul RichText
outlineElem.AppendChildLast(text);

// Tambahkan simpul OutlineElement
outline.AppendChildLast(outlineElem);

// Tambahkan simpul Outline
page.AppendChildLast(outline);

// Tambahkan simpul Halaman
doc.AppendChildLast(page);

// Simpan dokumen OneNote
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
doc.Save(dataDir);
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

Menunjukkan cara menyiapkan template untuk rapat mingguan.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Tags();

// Buat objek dari kelas Dokumen
var headerStyle = new ParagraphStyle() { FontName = "Calibri", FontSize = 16 };
var bodyStyle = new ParagraphStyle() { FontName = "Calibri", FontSize = 12 };

var d = new Document();
bool restartFlag = true;
var outline = d.AppendChildLast(new Page()
                                    {
                                        Title = new Title() { TitleText = new RichText() { Text = $"Weekly meeting {DateTime.Today:d}", ParagraphStyle = ParagraphStyle.Default } }
                                    })
               .AppendChildLast(new Outline() { VerticalOffset = 30, HorizontalOffset = 30 });

outline.AppendChildLast(new OutlineElement())
       .AppendChildLast(new RichText() { Text = "Important", ParagraphStyle = headerStyle });
foreach (var e in new[] { "First", "Second", "Third" })
{
    outline.AppendChildLast(new OutlineElement() { NumberList = CreateListNumberingStyle(bodyStyle, restartFlag) })
           .AppendChildLast(new RichText() { Text = e, ParagraphStyle = bodyStyle });
    restartFlag = false;
}

outline.AppendChildLast(new OutlineElement())
       .AppendChildLast(new RichText() { Text = "TO DO", ParagraphStyle = headerStyle, SpaceBefore = 15 });
restartFlag = true;
foreach (var e in new[] { "First", "Second", "Third" })
{
    outline.AppendChildLast(new OutlineElement() { NumberList = CreateListNumberingStyle(bodyStyle, restartFlag) })
           .AppendChildLast(new RichText() { Text = e, ParagraphStyle = bodyStyle, Tags = { NoteCheckBox.CreateBlueCheckBox() } });
    restartFlag = false;
}

d.Save(Path.Combine(dataDir, "meetingNotes.one"));
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

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [ITaggable](../itaggable/)
* ruang nama [Aspose.Note](../../aspose.note/)
* perakitan [Aspose.Note](../../)


