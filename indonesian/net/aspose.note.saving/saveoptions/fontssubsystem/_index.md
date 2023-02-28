---
title: SaveOptions.FontsSubsystem
second_title: Aspose.Note untuk Referensi .NET API
description: SaveOptions Properti. Mendapatkan atau menyetel pengaturan font untuk digunakan saat menyimpan
type: docs
weight: 10
url: /id/net/aspose.note.saving/saveoptions/fontssubsystem/
---
## SaveOptions.FontsSubsystem property

Mendapatkan atau menyetel pengaturan font untuk digunakan saat menyimpan

```csharp
public FontsSubsystem FontsSubsystem { get; set; }
```

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

* class [FontsSubsystem](../../../aspose.note.fonts/fontssubsystem/)
* class [SaveOptions](../)
* ruang nama [Aspose.Note.Saving](../../saveoptions/)
* perakitan [Aspose.Note](../../../)


