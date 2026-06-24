---
title: "TableCell.BackgroundColor"
second_title: "مرجع API لـ Aspose.Note لـ .NET"
description: "خاصية TableCell. يحصل أو يضبط لون الخلفية"
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

يظهر كيفية تعيين لون خلفية للخلية.

```csharp
// إنشاء كائن من الفئة Document
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

// تهيئة كائن الفئة Page
Page page = new Page();
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

### انظر أيضًا

* class [TableCell](../)
* namespace [Aspose.Note](../../tablecell/)
* assembly [Aspose.Note](../../../)


