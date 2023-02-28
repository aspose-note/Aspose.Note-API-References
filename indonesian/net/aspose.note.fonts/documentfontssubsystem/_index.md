---
title: Class DocumentFontsSubsystem
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.Fonts.DocumentFontsSubsystem kelas. Implementasi sederhana dari Aspose.Note.Fonts.FontsSubsystem. MengambilFontFamily objek dari OS.
type: docs
weight: 100
url: /id/net/aspose.note.fonts/documentfontssubsystem/
---
## DocumentFontsSubsystem class

Implementasi sederhana dari Aspose.Note.Fonts.FontsSubsystem. MengambilFontFamily objek dari OS.

```csharp
public class DocumentFontsSubsystem : FontsSubsystem
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor)(Dictionary&lt;string, string&gt;) | Menginisialisasi instance baru dari`DocumentFontsSubsystem` kelas. |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor_1)(Stream, Dictionary&lt;string, string&gt;) | Menginisialisasi instance baru dari`DocumentFontsSubsystem` kelas. |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor_2)(string, Dictionary&lt;string, string&gt;) | Menginisialisasi instance baru dari`DocumentFontsSubsystem` kelas. |

## Properti

| Nama | Keterangan |
| --- | --- |
| static [Default](../../aspose.note.fonts/documentfontssubsystem/default/) { get; set; } | Mendapat atau menyetel instance default statis. |
| [DefaultFont](../../aspose.note.fonts/fontssubsystem/defaultfont/) { get; } | Mendapat atau menyetel font default. |

## Metode

| Nama | Keterangan |
| --- | --- |
| static [UsingDefaultFont](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfont/)(string, Dictionary&lt;string, string&gt;) | Buat instance DocumentFontsSubsystem baru menggunakan nama font default yang ditentukan. |
| static [UsingDefaultFontFromFile](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/)(string, Dictionary&lt;string, string&gt;) | Buat instance DocumentFontsSubsystem baru menggunakan font dari file yang ditentukan sebagai default. |
| static [UsingDefaultFontFromStream](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream/)(Stream, Dictionary&lt;string, string&gt;) | Buat instance DocumentFontsSubsystem baru menggunakan font dari aliran yang ditentukan sebagai default. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(Stream) | Tambahkan font. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(string) | Tambahkan font. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(Stream, string) | Tambahkan font. |
| [AddFontSubstitution](../../aspose.note.fonts/fontssubsystem/addfontsubstitution/)(string, string) | Menambahkan penggantian font. |
| virtual [GetFontFamily](../../aspose.note.fonts/fontssubsystem/getfontfamily/)(string) | Mendapat jenis font. |
| [LoadFontsFromFolder](../../aspose.note.fonts/fontssubsystem/loadfontsfromfolder/)(string) | Memuat semua font TrueType dari folder tertentu ke koleksi internal. |

### Contoh

Menunjukkan cara menyimpan dokumen dalam format pdf menggunakan font default yang ditentukan.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Simpan dokumen sebagai PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

Menunjukkan cara menyimpan dokumen dalam format pdf menggunakan font default dari file.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Simpan dokumen sebagai PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

Menunjukkan cara menyimpan dokumen dalam format pdf menggunakan font default dari aliran.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Simpan dokumen sebagai PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### Lihat juga

* class [FontsSubsystem](../fontssubsystem/)
* ruang nama [Aspose.Note.Fonts](../../aspose.note.fonts/)
* perakitan [Aspose.Note](../../)


