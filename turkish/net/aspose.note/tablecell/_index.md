---
title: TableCell
second_title: Aspose.Note for .NET API Referansı
description: Bir tablo hücresini temsil eder.
type: docs
weight: 880
url: /tr/net/aspose.note/tablecell/
---
## TableCell class

Bir tablo hücresini temsil eder.

```csharp
public sealed class TableCell : CompositeNode<OutlineElement>
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [TableCell](tablecell#constructor)() | Yeni bir örneğini başlatır[`TableCell`](../tablecell) sınıf. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [BackgroundColor](../../aspose.note/tablecell/backgroundcolor) { get; set; } | Arka plan rengini alır veya ayarlar. |
| [Document](../../aspose.note/node/document) { get; } | Düğümün belgesini alır. |
| [FirstChild](../../aspose.note/compositenode`1/firstchild) { get; } |  |
| [IsComposite](../../aspose.note/compositenode`1/iscomposite) { get; } |  |
| [LastChild](../../aspose.note/compositenode`1/lastchild) { get; } |  |
| [LastModifiedTime](../../aspose.note/tablecell/lastmodifiedtime) { get; set; } | Son değiştirilme zamanını alır veya ayarlar. |
| [MaxWidth](../../aspose.note/tablecell/maxwidth) { get; } | Maksimum genişliği alır. |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | Aynı düğüm ağacı düzeyinde bir sonraki düğümü alır. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | Düğüm türünü alır. |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | Üst düğümü alır. |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | Aynı düğüm ağacı düzeyinde önceki düğümü alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| override [Accept](../../aspose.note/tablecell/accept)(DocumentVisitor) | Düğümün ziyaretçisini kabul eder. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildfirst)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildlast)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode`1/getchildnodes)() |  |
| [GetEnumerator](../../aspose.note/compositenode`1/getenumerator)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode`1/insertchild)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, IEnumerable&lt;OutlineElement&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, params OutlineElement[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode`1/removechild)(T1) |  |

### Örnekler

Bir tablonun hücrelerinden nasıl metin alınacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Tables();

// Belgeyi Aspose.Note'a yükleyin.
Document document = new Document(dataDir + "Sample1.one");

// Tablo düğümlerinin bir listesini alın
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // Tablo satırları arasında yineleme
    foreach (TableRow row in table)
    {
        // TableCell düğümlerinin listesini al
        // Tablo hücreleri arasında yineleme
        foreach (TableCell cell in row)
        {
            // Metni al
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // Çıktı ekranındaki metni yazdır
            Console.WriteLine(text);
        }
    }
}
```

Bir hücre için arka plan renginin nasıl ayarlanacağını gösterir.

```csharp
// Document sınıfının bir nesnesini oluşturun
Document doc = new Document();

// TableCell sınıf nesnesini başlat ve metin içeriğini ayarla
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
cell11.BackgroundColor = Color.Coral;

// TableRow sınıf nesnesini başlat
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

// Sayfa sınıfı nesnesini başlat
Page page = new Page(doc);
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

Etiketli yeni tablonun nasıl ekleneceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Tags();

// Document sınıfının bir nesnesini oluşturun
Document doc = new Document();

// Sayfa sınıfı nesnesini başlat
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// TableRow sınıf nesnesini başlat
TableRow row = new TableRow(doc);

// TableCell sınıf nesnesini başlat
TableCell cell = new TableCell(doc);

// Hücre içeriğini ekle
cell.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Single cell."));

// Satır düğümüne hücre ekle
row.AppendChildLast(cell);

// Tablo düğümünü başlat
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70 } }
              };

// Tabloya satır düğümü ekle
table.AppendChildLast(row);

// Bu tablo düğümüne etiket ekle
table.Tags.Add(NoteTag.CreateQuestionMark());

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// Tablo düğümü ekle
outlineElem.AppendChildLast(table);

// Anahat öğeleri ekle
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// OneNote belgesini kaydet
dataDir = dataDir + "AddTableNodeWithTag_out.one";
doc.Save(dataDir);
```

Kilitli sütunlu bir tablonun nasıl oluşturulacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Tables();

// Document sınıfının bir nesnesini oluşturun
Document doc = new Document();

// Sayfa sınıfı nesnesini başlat
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// TableRow sınıf nesnesini başlat
TableRow row1 = new TableRow(doc);

// TableCell sınıf nesnesini başlat ve metin içeriğini ayarla
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
row1.AppendChildLast(cell11);

// TableRow sınıf nesnesini başlat
TableRow row2 = new TableRow(doc);

// TableCell sınıf nesnesini başlat ve metin içeriğini ayarla
TableCell cell21 = new TableCell(doc);
cell21.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Long   text    with    several   words and    spaces."));
row2.AppendChildLast(cell21);

// Tablo sınıfı nesnesini başlat
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70, LockedWidth = true } }
              };

// Satır ekle
table.AppendChildLast(row1);
table.AppendChildLast(row2);

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// Tablo düğümü ekle
outlineElem.AppendChildLast(table);

// Anahat öğesi düğümü ekle
outline.AppendChildLast(outlineElem);

// Anahat düğümü ekle
page.AppendChildLast(outline);

// Sayfa düğümü ekle
doc.AppendChildLast(page);
dataDir = dataDir + "CreateTableWithLockedColumns_out.one";
doc.Save(dataDir);
```

Yeni bir tablonun nasıl oluşturulacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Tables();

// Document sınıfının bir nesnesini oluşturun
Document doc = new Document();

// Sayfa sınıfı nesnesini başlat
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// TableRow sınıf nesnesini başlat
TableRow row1 = new TableRow(doc);

// TableCell sınıf nesnelerini başlat
TableCell cell11 = new TableCell(doc);
TableCell cell12 = new TableCell(doc);
TableCell cell13 = new TableCell(doc);

// Tablo hücresine anahat öğeleri ekle
cell11.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.1"));
cell12.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.2"));
cell13.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.3"));

// Tablo hücrelerini satırlara
row1.AppendChildLast(cell11);
row1.AppendChildLast(cell12);
row1.AppendChildLast(cell13);

// TableRow sınıf nesnesini başlat
TableRow row2 = new TableRow(doc);

// TableCell sınıf nesnelerini başlat
TableCell cell21 = new TableCell(doc);
TableCell cell22 = new TableCell(doc);
TableCell cell23 = new TableCell(doc);

// Tablo hücresine anahat öğeleri ekle
cell21.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.1"));
cell22.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.2"));
cell23.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.3"));

// Tablo hücrelerini satırlara ekle
row2.AppendChildLast(cell21);
row2.AppendChildLast(cell22);
row2.AppendChildLast(cell23);

// Tablo sınıfı nesnesini başlat ve sütun genişliklerini ayarla
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 200 }, new TableColumn { Width = 200 }, new TableColumn { Width = 200 } }
              };

// Tablo satırlarını tabloya ekle
table.AppendChildLast(row1);
table.AppendChildLast(row2);

// Outline nesnesini başlat
Outline outline = new Outline(doc);

// OutlineElement nesnesini başlat
OutlineElement outlineElem = new OutlineElement(doc);

// Öğe düğümünü ana hatlarıyla belirtmek için tablo ekle
outlineElem.AppendChildLast(table);

// Anahat için anahat öğesi ekle
outline.AppendChildLast(outlineElem);

// Sayfa düğümüne anahat ekle
page.AppendChildLast(outline);

// Belge düğümüne sayfa ekle
doc.AppendChildLast(page);
dataDir = dataDir + "InsertTable_out.one";
doc.Save(dataDir);
```

### Ayrıca bakınız

* class [CompositeNode&lt;T&gt;](../compositenode-1)
* class [OutlineElement](../outlineelement)
* ad alanı [Aspose.Note](../../aspose.note)
* toplantı [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
