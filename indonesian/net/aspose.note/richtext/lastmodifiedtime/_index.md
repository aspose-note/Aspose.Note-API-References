---
title: RichText.LastModifiedTime
second_title: Aspose.Note untuk Referensi .NET API
description: RichText Properti. Mendapatkan atau menyetel waktu modifikasi terakhir.
type: docs
weight: 30
url: /id/net/aspose.note/richtext/lastmodifiedtime/
---
## RichText.LastModifiedTime property

Mendapatkan atau menyetel waktu modifikasi terakhir.

```csharp
public DateTime LastModifiedTime { get; set; }
```

### Contoh

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

### Lihat juga

* class [RichText](../)
* ruang nama [Aspose.Note](../../richtext/)
* perakitan [Aspose.Note](../../../)


