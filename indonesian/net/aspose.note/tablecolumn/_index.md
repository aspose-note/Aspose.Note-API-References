---
title: Class TableColumn
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.TableColumn kelas. Merupakan kolom tabel.
type: docs
weight: 920
url: /id/net/aspose.note/tablecolumn/
---
## TableColumn class

Merupakan kolom tabel.

```csharp
public sealed class TableColumn
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [TableColumn](tablecolumn/)() | Konstruktor default. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [LockedWidth](../../aspose.note/tablecolumn/lockedwidth/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah kolom tabel memiliki lebar yang dikunci dan tidak mengubah ukuran secara otomatis agar pas dengan konten tabel. Secara default, lebar kolom tidak dikunci. |
| [Width](../../aspose.note/tablecolumn/width/) { get; set; } | Mendapat atau mengatur lebar. |

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

Menunjukkan cara menambahkan tabel baru dengan tag.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Tags();

// Buat objek dari kelas Dokumen
Document doc = new Document();

// Inisialisasi objek kelas Halaman
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inisialisasi objek kelas TableRow
TableRow row = new TableRow(doc);

// Inisialisasi objek kelas TableCell
TableCell cell = new TableCell(doc);

// Sisipkan konten sel
cell.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Single cell."));

// Tambahkan sel ke simpul baris
row.AppendChildLast(cell);

// Inisialisasi simpul tabel
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70 } }
              };

// Masukkan simpul baris ke dalam tabel
table.AppendChildLast(row);

// Tambahkan tag ke simpul tabel ini
table.Tags.Add(NoteTag.CreateQuestionMark());

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// Tambahkan simpul tabel
outlineElem.AppendChildLast(table);

// Tambahkan elemen kerangka
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// Simpan dokumen OneNote
dataDir = dataDir + "AddTableNodeWithTag_out.one";
doc.Save(dataDir);
```

Menunjukkan cara membuat tabel dengan kolom terkunci.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Tables();

// Buat objek dari kelas Dokumen
Document doc = new Document();

// Inisialisasi objek kelas Halaman
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inisialisasi objek kelas TableRow
TableRow row1 = new TableRow(doc);

// Inisialisasi objek kelas TableCell dan atur konten teks
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
row1.AppendChildLast(cell11);

// Inisialisasi objek kelas TableRow
TableRow row2 = new TableRow(doc);

// Inisialisasi objek kelas TableCell dan atur konten teks
TableCell cell21 = new TableCell(doc);
cell21.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Long   text    with    several   words and    spaces."));
row2.AppendChildLast(cell21);

// Inisialisasi objek kelas Tabel
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70, LockedWidth = true } }
              };

// Tambahkan baris
table.AppendChildLast(row1);
table.AppendChildLast(row2);

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// Tambahkan simpul tabel
outlineElem.AppendChildLast(table);

// Tambahkan simpul elemen kerangka
outline.AppendChildLast(outlineElem);

// Tambahkan simpul kerangka
page.AppendChildLast(outline);

// Tambahkan simpul halaman
doc.AppendChildLast(page);
dataDir = dataDir + "CreateTableWithLockedColumns_out.one";
doc.Save(dataDir);
```

Menunjukkan cara membuat tabel baru.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Tables();

// Buat objek dari kelas Dokumen
Document doc = new Document();

// Inisialisasi objek kelas Halaman
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inisialisasi objek kelas TableRow
TableRow row1 = new TableRow(doc);

// Inisialisasi objek kelas TableCell
TableCell cell11 = new TableCell(doc);
TableCell cell12 = new TableCell(doc);
TableCell cell13 = new TableCell(doc);

// Tambahkan elemen kerangka di sel tabel
cell11.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.1"));
cell12.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.2"));
cell13.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.3"));

// Tabel sel ke baris
row1.AppendChildLast(cell11);
row1.AppendChildLast(cell12);
row1.AppendChildLast(cell13);

// Inisialisasi objek kelas TableRow
TableRow row2 = new TableRow(doc);

// inisialisasi objek kelas TableCell
TableCell cell21 = new TableCell(doc);
TableCell cell22 = new TableCell(doc);
TableCell cell23 = new TableCell(doc);

// Tambahkan elemen kerangka di sel tabel
cell21.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.1"));
cell22.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.2"));
cell23.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.3"));

// Tambahkan sel tabel ke baris
row2.AppendChildLast(cell21);
row2.AppendChildLast(cell22);
row2.AppendChildLast(cell23);

// Inisialisasi objek kelas Tabel dan atur lebar kolom
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 200 }, new TableColumn { Width = 200 }, new TableColumn { Width = 200 } }
              };

// Tambahkan baris tabel ke tabel
table.AppendChildLast(row1);
table.AppendChildLast(row2);

// Inisialisasi objek Outline
Outline outline = new Outline(doc);

// Inisialisasi objek OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Tambahkan tabel ke simpul elemen kerangka
outlineElem.AppendChildLast(table);

// Tambahkan elemen outline ke outline
outline.AppendChildLast(outlineElem);

// Tambahkan kerangka ke simpul halaman
page.AppendChildLast(outline);

// Tambahkan halaman ke simpul dokumen
doc.AppendChildLast(page);
dataDir = dataDir + "InsertTable_out.one";
doc.Save(dataDir);
```

### Lihat juga

* ruang nama [Aspose.Note](../../aspose.note/)
* perakitan [Aspose.Note](../../)


