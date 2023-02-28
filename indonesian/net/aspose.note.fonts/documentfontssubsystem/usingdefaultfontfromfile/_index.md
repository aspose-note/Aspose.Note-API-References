---
title: DocumentFontsSubsystem.UsingDefaultFontFromFile
second_title: Aspose.Note untuk Referensi .NET API
description: DocumentFontsSubsystem metode. Buat instance DocumentFontsSubsystem baru menggunakan font dari file yang ditentukan sebagai default.
type: docs
weight: 40
url: /id/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/
---
## DocumentFontsSubsystem.UsingDefaultFontFromFile method

Buat instance DocumentFontsSubsystem baru menggunakan font dari file yang ditentukan sebagai default.

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromFile(string filePath, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| filePath | String | File yang berisi nama font default. |
| fontsSubstitutions | Dictionary`2 | Penggantian font. |

### Nilai Pengembalian

Itu[`DocumentFontsSubsystem`](../) .

### Contoh

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

### Lihat juga

* class [DocumentFontsSubsystem](../)
* ruang nama [Aspose.Note.Fonts](../../documentfontssubsystem/)
* perakitan [Aspose.Note](../../../)


