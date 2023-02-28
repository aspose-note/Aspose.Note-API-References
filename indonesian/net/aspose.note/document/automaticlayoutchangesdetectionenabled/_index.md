---
title: Document.AutomaticLayoutChangesDetectionEnabled
second_title: Aspose.Note untuk Referensi .NET API
description: Document Properti. Mendapat atau menetapkan nilai yang menunjukkan apakah Aspose.Note melakukan deteksi perubahan tata letak secara otomatis. Nilai default adalahBENAR .
type: docs
weight: 20
url: /id/net/aspose.note/document/automaticlayoutchangesdetectionenabled/
---
## Document.AutomaticLayoutChangesDetectionEnabled property

Mendapat atau menetapkan nilai yang menunjukkan apakah Aspose.Note melakukan deteksi perubahan tata letak secara otomatis. Nilai default adalah`BENAR` .

```csharp
public bool AutomaticLayoutChangesDetectionEnabled { get; set; }
```

### Contoh

Menunjukkan cara menyimpan dokumen dalam berbagai format.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Inisialisasi Dokumen baru
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// Inisialisasi Halaman baru
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Gaya default untuk semua teks dalam dokumen.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Tambahkan simpul halaman
doc.AppendChildLast(page);

// Simpan dokumen OneNote dalam berbagai format, atur ukuran font teks dan deteksi perubahan tata letak secara manual.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

### Lihat juga

* class [Document](../)
* ruang nama [Aspose.Note](../../document/)
* perakitan [Aspose.Note](../../../)


