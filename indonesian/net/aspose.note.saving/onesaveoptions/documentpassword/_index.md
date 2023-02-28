---
title: OneSaveOptions.DocumentPassword
second_title: Aspose.Note untuk Referensi .NET API
description: OneSaveOptions Properti. Mendapatkan atau menyetel kata sandi untuk mengenkripsi konten dokumen.
type: docs
weight: 20
url: /id/net/aspose.note.saving/onesaveoptions/documentpassword/
---
## OneSaveOptions.DocumentPassword property

Mendapatkan atau menyetel kata sandi untuk mengenkripsi konten dokumen.

```csharp
public string DocumentPassword { get; set; }
```

### Contoh

Menunjukkan cara menyimpan dokumen dengan enkripsi.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

### Lihat juga

* class [OneSaveOptions](../)
* ruang nama [Aspose.Note.Saving](../../onesaveoptions/)
* perakitan [Aspose.Note](../../../)


