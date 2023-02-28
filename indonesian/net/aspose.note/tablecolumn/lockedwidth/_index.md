---
title: TableColumn.LockedWidth
second_title: Aspose.Note untuk Referensi .NET API
description: TableColumn Properti. Mendapat atau menetapkan nilai yang menunjukkan apakah kolom tabel memiliki lebar yang dikunci dan tidak mengubah ukuran secara otomatis agar pas dengan konten tabel. Secara default lebar kolom tidak dikunci.
type: docs
weight: 20
url: /id/net/aspose.note/tablecolumn/lockedwidth/
---
## TableColumn.LockedWidth property

Mendapat atau menetapkan nilai yang menunjukkan apakah kolom tabel memiliki lebar yang dikunci dan tidak mengubah ukuran secara otomatis agar pas dengan konten tabel. Secara default, lebar kolom tidak dikunci.

```csharp
public bool LockedWidth { get; set; }
```

### Contoh

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

### Lihat juga

* class [TableColumn](../)
* ruang nama [Aspose.Note](../../tablecolumn/)
* perakitan [Aspose.Note](../../../)


