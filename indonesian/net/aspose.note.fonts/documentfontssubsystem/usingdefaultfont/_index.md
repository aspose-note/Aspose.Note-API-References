---
title: DocumentFontsSubsystem.UsingDefaultFont
second_title: Aspose.Note untuk Referensi .NET API
description: DocumentFontsSubsystem metode. Buat instance DocumentFontsSubsystem baru menggunakan nama font default yang ditentukan.
type: docs
weight: 30
url: /id/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfont/
---
## DocumentFontsSubsystem.UsingDefaultFont method

Buat instance DocumentFontsSubsystem baru menggunakan nama font default yang ditentukan.

```csharp
public static DocumentFontsSubsystem UsingDefaultFont(string defaultFontName, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| defaultFontName | String | Nama font default. |
| fontsSubstitutions | Dictionary`2 | Penggantian font. |

### Nilai Pengembalian

Itu[`DocumentFontsSubsystem`](../) .

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

### Lihat juga

* class [DocumentFontsSubsystem](../)
* ruang nama [Aspose.Note.Fonts](../../documentfontssubsystem/)
* perakitan [Aspose.Note](../../../)


