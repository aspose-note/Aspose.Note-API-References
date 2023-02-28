---
title: TableCell.BackgroundColor
second_title: Aspose.Note untuk Referensi .NET API
description: TableCell Properti. Mendapat atau mengatur warna latar belakang.
type: docs
weight: 20
url: /id/net/aspose.note/tablecell/backgroundcolor/
---
## TableCell.BackgroundColor property

Mendapat atau mengatur warna latar belakang.

```csharp
public Color BackgroundColor { get; set; }
```

### Contoh

Memperlihatkan cara menyetel warna latar belakang untuk sel.

```csharp
// Buat objek dari kelas Dokumen
Document doc = new Document();

// Inisialisasi objek kelas TableCell dan atur konten teks
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
cell11.BackgroundColor = Color.Coral;

// Inisialisasi objek kelas TableRow
TableRow row = new TableRow(doc);
row.AppendChildLast(cell11);

Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn() { Width = 200 } }
              };
table.AppendChildLast(row);

OutlineElement oe = new OutlineElement(doc);
oe.AppendChildLast(table);

Outline o = new Outline(doc);
o.AppendChildLast(oe);

// Inisialisasi objek kelas Halaman
Page page = new Page(doc);
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

### Lihat juga

* class [TableCell](../)
* ruang nama [Aspose.Note](../../tablecell/)
* perakitan [Aspose.Note](../../../)


