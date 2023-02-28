---
title: Style.IsBold
second_title: Aspose.Note untuk Referensi .NET API
description: Style Properti. Mendapat atau menetapkan nilai yang menunjukkan apakah gaya teks dicetak tebal.
type: docs
weight: 60
url: /id/net/aspose.note/style/isbold/
---
## Style.IsBold property

Mendapat atau menetapkan nilai yang menunjukkan apakah gaya teks dicetak tebal.

```csharp
public bool IsBold { get; set; }
```

### Contoh

Mari kita tekankan judul halaman di antara header lainnya dengan memperbesar ukuran font.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Muat dokumen ke Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Ulangi judul halaman.
foreach (var title in document.Select(e => e.Title.TitleText))
{
    title.ParagraphStyle.FontSize = 24;
    title.ParagraphStyle.IsBold = true;

    foreach (var run in title.TextRuns)
    {
        run.Style.FontSize = 24;
        run.Style.IsBold = true;
    }
}

document.Save(Path.Combine(dataDir, "ChangePageTitleStyle.pdf"));
```

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

* class [Style](../)
* ruang nama [Aspose.Note](../../style/)
* perakitan [Aspose.Note](../../../)


