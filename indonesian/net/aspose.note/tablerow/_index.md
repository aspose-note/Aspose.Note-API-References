---
title: Class TableRow
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.TableRow kelas. Merupakan baris tabel.
type: docs
weight: 930
url: /id/net/aspose.note/tablerow/
---
## TableRow class

Merupakan baris tabel.

```csharp
public sealed class TableRow : CompositeNode<TableCell>
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [TableRow](tablerow/#constructor)() | Menginisialisasi instance baru dari`TableRow` kelas. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Mendapat dokumen dari node. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [LastModifiedTime](../../aspose.note/tablerow/lastmodifiedtime/) { get; set; } | Mendapatkan atau menyetel waktu modifikasi terakhir. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Mendapat node berikutnya pada tingkat pohon node yang sama. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Mendapat tipe node. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Mendapat simpul induk. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Mendapat simpul sebelumnya pada tingkat pohon simpul yang sama. |

## Metode

| Nama | Keterangan |
| --- | --- |
| override [Accept](../../aspose.note/tablerow/accept/)(DocumentVisitor) | Menerima pengunjung node. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;TableCell&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params TableCell[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |

### Contoh

Menunjukkan cara mendapatkan teks dari setiap baris tabel.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Tables();

// Muat dokumen ke Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Dapatkan daftar node tabel
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // Iterasi melalui baris tabel
    foreach (TableRow row in table)
    {
        // Mengambil teks
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // Cetak teks pada layar keluaran
        Console.WriteLine(text);
    }
}
```

Menunjukkan cara mendapatkan teks dari sel tabel.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Tables();

// Muat dokumen ke Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Dapatkan daftar node tabel
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // Iterasi melalui baris tabel
    foreach (TableRow row in table)
    {
        // Dapatkan daftar node TableCell
        // Iterasi melalui sel tabel
        foreach (TableCell cell in row)
        {
            // Mengambil teks
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // Cetak teks pada layar keluaran
            Console.WriteLine(text);
        }
    }
}
```

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

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* class [TableCell](../tablecell/)
* ruang nama [Aspose.Note](../../aspose.note/)
* perakitan [Aspose.Note](../../)


