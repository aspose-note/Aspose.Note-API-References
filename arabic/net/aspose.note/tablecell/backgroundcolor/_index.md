---
title: "TableCell.BackgroundColor"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "TableCell خاصية. يحصل على أو يضبط لون الخلفية"
type: docs
weight: 20
url: /ar/net/aspose.note/tablecell/backgroundcolor/
---
## TableCell.BackgroundColor property

يحصل أو يضبط لون الخلفية.

```csharp
public Color BackgroundColor { get; set; }
```

## أمثلة

يوضح كيفية تعيين لون خلفية لخلية.

```csharp
// إنشاء كائن من فئة Document
Document doc = new Document();

// تهيئة كائن فئة TableCell وتعيين محتوى النص
TableCell cell11 = new TableCell();
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText("Small text"));
cell11.BackgroundColor = Color.Coral;

// تهيئة كائن فئة TableRow
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

// تهيئة كائن فئة Page
Page page = new Page();
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

### انظر أيضًا

* class [TableCell](../)
* namespace [Aspose.Note](../../tablecell/)
* assembly [Aspose.Note](../../../)


