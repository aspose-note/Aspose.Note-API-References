---
title: DocumentFontsSubsystem.UsingDefaultFontFromStream
second_title: Aspose.Note untuk Referensi .NET API
description: DocumentFontsSubsystem metode. Buat instance DocumentFontsSubsystem baru menggunakan font dari aliran yang ditentukan sebagai default.
type: docs
weight: 50
url: /id/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream/
---
## DocumentFontsSubsystem.UsingDefaultFontFromStream method

Buat instance DocumentFontsSubsystem baru menggunakan font dari aliran yang ditentukan sebagai default.

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromStream(Stream defaultFontStream, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| defaultFontStream | Stream | Aliran yang berisi nama font default. |
| fontsSubstitutions | Dictionary`2 | Penggantian font. |

### Nilai Pengembalian

Itu[`DocumentFontsSubsystem`](../) .

### Contoh

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

* class [DocumentFontsSubsystem](../)
* ruang nama [Aspose.Note.Fonts](../../documentfontssubsystem/)
* perakitan [Aspose.Note](../../../)


