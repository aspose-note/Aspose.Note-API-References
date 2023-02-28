---
title: Class HtmlSaveOptions
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.Saving.HtmlSaveOptions kelas. Memungkinkan untuk menentukan opsi tambahan saat menyimpan dokumen ke format HTML.
type: docs
weight: 700
url: /id/net/aspose.note.saving/htmlsaveoptions/
---
## HtmlSaveOptions class

Memungkinkan untuk menentukan opsi tambahan saat menyimpan dokumen ke format HTML.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions/)() | Konstruktor default. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [CssPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/cssperpagegeneration/) { get; set; } | Mendapatkan atau menyetel apakah file StyleSheet akan dibuat untuk setiap halaman baru secara terpisah. |
| [CssSavingCallback](../../aspose.note.saving/htmlsaveoptions/csssavingcallback/) { get; set; } | Mendapat atau menyetel callback yang dipanggil untuk membuat sumber daya untuk menyimpan CSS. |
| [DocumentPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/documentperpagegeneration/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah pembuatan dokumen per halaman diaktifkan. |
| [ExportCss](../../aspose.note.saving/htmlsaveoptions/exportcss/) { get; set; } | Mendapat atau mengatur cara css diekspor. |
| [ExportFonts](../../aspose.note.saving/htmlsaveoptions/exportfonts/) { get; set; } | Mendapatkan atau menyetel cara font diekspor. |
| [ExportImages](../../aspose.note.saving/htmlsaveoptions/exportimages/) { get; set; } | Mendapat atau mengatur cara gambar diekspor. |
| [FontFaceTypes](../../aspose.note.saving/htmlsaveoptions/fontfacetypes/) { get; set; } | Mendapat atau menyetel jenis tampilan font. |
| [FontSavingCallback](../../aspose.note.saving/htmlsaveoptions/fontsavingcallback/) { get; set; } | Mendapat atau menyetel panggilan balik yang dipanggil untuk membuat sumber daya untuk menyimpan font. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | Mendapatkan atau menyetel pengaturan font untuk digunakan saat menyimpan |
| [ImageSavingCallback](../../aspose.note.saving/htmlsaveoptions/imagesavingcallback/) { get; set; } | Mendapat atau menyetel panggilan balik yang dipanggil untuk membuat sumber daya untuk menyimpan gambar. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | Mendapat atau mengatur jumlah halaman yang akan disimpan. Secara default adalahMaxValue yang berarti semua halaman dokumen akan dirender. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | Mendapat atau menetapkan indeks halaman pertama yang akan disimpan. Secara default adalah 0. |
| [PageSavingCallback](../../aspose.note.saving/htmlsaveoptions/pagesavingcallback/) { get; set; } | Mendapat atau menyetel panggilan balik yang dipanggil untuk membuat sumber daya ke halaman penyimpanan. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | Mendapatkan format penyimpanan dokumen. |

### Contoh

Menunjukkan cara menyimpan dokumen dalam format html dengan menyimpan semua sumber daya (css/font/gambar) ke file terpisah.

```csharp
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

var options = new HtmlSaveOptions()
             {
                 ExportCss = ResourceExportType.ExportAsStream,
                 ExportFonts = ResourceExportType.ExportAsStream,
                 ExportImages = ResourceExportType.ExportAsStream,
                 FontFaceTypes = FontFaceType.Ttf
             };
document.Save(dataDir + "document_out.html", options);
```

Menunjukkan cara menyimpan dokumen ke aliran dalam format html dengan menyematkan semua sumber daya (css/font/gambar).

```csharp
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

var options = new HtmlSaveOptions()
             {
                 ExportCss = ResourceExportType.ExportEmbedded,
                 ExportFonts = ResourceExportType.ExportEmbedded,
                 ExportImages = ResourceExportType.ExportEmbedded,
                 FontFaceTypes = FontFaceType.Ttf
             };

var r = new MemoryStream();
document.Save(r, options);
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

Menunjukkan cara menyimpan dokumen dalam format html dengan menyimpan semua sumber daya (css/font/gambar) dengan menggunakan panggilan balik yang ditentukan pengguna.

```csharp
// Kode di bawah membuat folder 'documentFolder' yang berisi document.html, folder 'css' dengan file 'style.css', folder 'images' dengan gambar dan folder 'fonts' dengan font.
// File 'style.css' akan berisi string berikut "/* Baris ini ditambahkan untuk streaming secara manual oleh pengguna */"
var savingCallbacks = new UserSavingCallbacks()
                          {
                              RootFolder = "documentFolder",
                              CssFolder = "css",
                              KeepCssStreamOpened = true,
                              ImagesFolder = "images",
                              FontsFolder = "fonts"
                          };
var options = new HtmlSaveOptions
              {
                  FontFaceTypes = FontFaceType.Ttf,
                  CssSavingCallback = savingCallbacks,
                  FontSavingCallback = savingCallbacks,
                  ImageSavingCallback = savingCallbacks
              };

if (!Directory.Exists(savingCallbacks.RootFolder))
{
    Directory.CreateDirectory(savingCallbacks.RootFolder);
}

string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

using (var stream = File.Create(Path.Combine(savingCallbacks.RootFolder, "document.html")))
{
    document.Save(stream, options);
}

using (var writer = new StreamWriter(savingCallbacks.CssStream))
{
    writer.WriteLine();
    writer.WriteLine("/* This line is appended to stream manually by user */");
}
```

### Lihat juga

* class [SaveOptions](../saveoptions/)
* ruang nama [Aspose.Note.Saving](../../aspose.note.saving/)
* perakitan [Aspose.Note](../../)


