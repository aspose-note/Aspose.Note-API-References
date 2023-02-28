---
title: Style.Highlight
second_title: Aspose.Note untuk Referensi .NET API
description: Style Properti. Mendapat atau menyetel warna sorotan.
type: docs
weight: 50
url: /id/net/aspose.note/style/highlight/
---
## Style.Highlight property

Mendapat atau menyetel warna sorotan.

```csharp
public Color Highlight { get; set; }
```

### Contoh

Menunjukkan cara mengubah gaya teks.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Muat dokumen ke Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Dapatkan node RichText tertentu
RichText richText = document.GetChildNodes<RichText>().First();

foreach (var run in richText.TextRuns)
{
    // Atur warna font
    run.Style.FontColor = Color.Yellow;

    // Tetapkan warna sorotan
    run.Style.Highlight = Color.Blue;

    // Tetapkan ukuran font
    run.Style.FontSize = 20;
}
```

Menunjukkan cara membuat tabel yang memiliki teks dengan berbagai gaya.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

var headerText = new RichText() { ParagraphStyle = new ParagraphStyle() { FontSize = 18, IsBold = true }, Alignment = HorizontalAlignment.Center }
                    .Append("Super contest for suppliers.");

var page = new Page();
var outline = page.AppendChildLast(new Outline() { HorizontalOffset = 50 });
outline.AppendChildLast(new OutlineElement()).AppendChildLast(headerText);

// Ringkasan teks sebelum tabel
var bodyTextHeader = outline.AppendChildLast(new OutlineElement()).AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default });
bodyTextHeader.Append("This is the final ranking of proposals got from our suppliers.");

var ranking = outline.AppendChildLast(new OutlineElement()).AppendChildLast(new Table());
var headerRow = ranking.AppendChildFirst(new TableRow());

var headerStyle = ParagraphStyle.Default;
headerStyle.IsBold = true;

// Mari tambahkan satu set kolom dan baris header
var backGroundColor = Color.LightGray;
foreach (var header in new[] { "Supplier", "Contacts", "Score A", "Score B", "Score C", "Final score", "Attached materials", "Comments" })
{
    ranking.Columns.Add(new TableColumn());
    headerRow.AppendChildLast(new TableCell() { BackgroundColor = backGroundColor })
             .AppendChildLast(new OutlineElement())
             .AppendChildLast(new RichText() { ParagraphStyle = headerStyle })
                .Append(header);
}

// Ayo 5 baris kosong. Baris memiliki warna latar belakang yang saling bertukar
for (int i = 0; i < 5; i++)
{
    backGroundColor = backGroundColor.IsEmpty ? Color.LightGray : Color.Empty;

    var row = ranking.AppendChildLast(new TableRow());
    for (int j = 0; j < ranking.Columns.Count(); j++)
    {
        row.AppendChildLast(new TableCell() { BackgroundColor = backGroundColor })
           .AppendChildLast(new OutlineElement())
           .AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default });
    }
}

// Mari tambahkan beberapa template untuk konten di kolom 'Kontak'
foreach (var row in ranking.Skip(1))
{
    var contactsCell = row.ElementAt(1);
    contactsCell.AppendChildLast(new OutlineElement())
                .AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default })
                    .Append("Web: ").Append("link", new TextStyle() { HyperlinkAddress = "www.link.com", IsHyperlink = true });
    contactsCell.AppendChildLast(new OutlineElement())
                .AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default })
                    .Append("E-mail: ").Append("mail", new TextStyle() { HyperlinkAddress = "mailto:hi@link.com", IsHyperlink = true });
}

var d = new Document();
d.AppendChildLast(page);
d.Save(Path.Combine(dataDir, "ComposeTable_out.one"));
```

### Lihat juga

* class [Style](../)
* ruang nama [Aspose.Note](../../style/)
* perakitan [Aspose.Note](../../../)


