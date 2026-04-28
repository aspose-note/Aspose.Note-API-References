---
title: TableCell.BackgroundColor
second_title: Aspose.Note for .NET API Referansı
description: TableCell mülk. Arka plan rengini alır veya ayarlar.
type: docs
weight: 20
url: /tr/net/aspose.note/tablecell/backgroundcolor/
---
## TableCell.BackgroundColor property

Arka plan rengini alır veya ayarlar.

```csharp
public Color BackgroundColor { get; set; }
```

### Örnekler

Bir hücre için arka plan renginin nasıl ayarlanacağını gösterir.

```csharp
// Document sınıfından bir nesne oluşturun
Document doc = new Document();

// TableCell sınıf nesnesini başlat ve metin içeriğini ayarla
TableCell cell11 = new TableCell();
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
cell11.BackgroundColor = Color.Coral;

// TableRow sınıf nesnesini başlat
TableRow row = new TableRow();
row.AppendChildLast(cell11);

Table table = new Table()
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn() { Width = 200 } }
              };
table.AppendChildLast(row);

OutlineElement oe = new OutlineElement();
oe.AppendChildLast(table);

Outline o = new Outline();
o.AppendChildLast(oe);

// Sayfa sınıfı nesnesini başlat
Page page = new Page();
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

### Ayrıca bakınız

* class [TableCell](../)
* ad alanı [Aspose.Note](../../tablecell/)
* toplantı [Aspose.Note](../../../)


