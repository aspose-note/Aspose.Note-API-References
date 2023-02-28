---
title: SaveOptions.PageIndex
second_title: Aspose.Note untuk Referensi .NET API
description: SaveOptions Properti. Mendapat atau menetapkan indeks halaman pertama yang akan disimpan. Secara default adalah 0.
type: docs
weight: 30
url: /id/net/aspose.note.saving/saveoptions/pageindex/
---
## SaveOptions.PageIndex property

Mendapat atau menetapkan indeks halaman pertama yang akan disimpan. Secara default adalah 0.

```csharp
public int PageIndex { get; set; }
```

### Contoh

Menunjukkan cara menyimpan dokumen dalam format png.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Inisialisasi objek ImageSaveOptions 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // Tetapkan indeks halaman
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// Simpan dokumen sebagai PNG.
oneFile.Save(dataDir, opts);
```

Menampilkan cara menyimpan dokumen dalam format pdf.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Inisialisasi objek PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Tetapkan indeks halaman dari halaman pertama yang akan disimpan
                              PageIndex = 0,

                              // Setel jumlah halaman
                              PageCount = 1,
                          };

// Simpan dokumen sebagai PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Menunjukkan cara menyimpan dokumen dalam format pdf menggunakan pengaturan khusus.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Inisialisasi objek PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Gunakan kompresi Jpeg
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Kualitas untuk kompresi JPEG
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
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

Memperlihatkan cara membuat dokumen dengan teks kaya yang diformat.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Buat objek dari kelas Dokumen
Document doc = new Document();

// Inisialisasi objek kelas Halaman
Page page = new Page();

// Inisialisasi objek kelas Judul
Title title = new Title();

// Inisialisasi objek kelas TextStyle dan atur properti pemformatan
ParagraphStyle defaultTextStyle = new ParagraphStyle
                                      {
                                          FontColor = Color.Black,
                                          FontName = "Arial",
                                          FontSize = 10
                                      };

RichText titleText = new RichText() { ParagraphStyle = defaultTextStyle }.Append("Title!");
Outline outline = new Outline()
                      {
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };
OutlineElement outlineElem = new OutlineElement();

TextStyle textStyleForHelloWord = new TextStyle
                                      {
                                          FontColor = Color.Red,
                                          FontName = "Arial",
                                          FontSize = 10,
                                      };

TextStyle textStyleForOneNoteWord = new TextStyle
                                        {
                                            FontColor = Color.Green,
                                            FontName = "Calibri",
                                            FontSize = 10,
                                            IsItalic = true,
                                        };

TextStyle textStyleForTextWord = new TextStyle
                                     {
                                         FontColor = Color.Blue,
                                         FontName = "Arial",
                                         FontSize = 15,
                                         IsBold = true,
                                         IsItalic = true,
                                     };

RichText text = new RichText() { ParagraphStyle = defaultTextStyle }
                    .Append("Hello", textStyleForHelloWord)
                    .Append(" OneNote", textStyleForOneNoteWord)
                    .Append(" text", textStyleForTextWord)
                    .Append("!", TextStyle.Default);

title.TitleText = titleText;

// Tetapkan judul halaman
page.Title = title;

// Tambahkan simpul RichText
outlineElem.AppendChildLast(text);

// Tambahkan simpul OutlineElement
outline.AppendChildLast(outlineElem);

// Tambahkan simpul Outline
page.AppendChildLast(outline);

// Tambahkan simpul Halaman
doc.AppendChildLast(page);

// Simpan dokumen OneNote
dataDir = dataDir + "CreateDocWithFormattedRichText_out.one";
doc.Save(dataDir);
```

### Lihat juga

* class [SaveOptions](../)
* ruang nama [Aspose.Note.Saving](../../saveoptions/)
* perakitan [Aspose.Note](../../../)


