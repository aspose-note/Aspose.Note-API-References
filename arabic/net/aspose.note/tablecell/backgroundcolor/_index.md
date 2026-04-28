---
title: TableCell.BackgroundColor
second_title: Aspose.Note لمرجع NET API
description: TableCell ملكية. الحصول على لون الخلفية أو تعيينه.
type: docs
weight: 20
url: /ar/net/aspose.note/tablecell/backgroundcolor/
---
## TableCell.BackgroundColor property

الحصول على لون الخلفية أو تعيينه.

```csharp
public Color BackgroundColor { get; set; }
```

### أمثلة

يوضح كيفية تعيين لون الخلفية لخلية.

```csharp
// إنشاء كائن من فئة المستند
Document doc = new Document();

// تهيئة كائن فئة TableCell وتعيين محتوى النص
TableCell cell11 = new TableCell();
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
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

// تهيئة كائن فئة الصفحة
Page page = new Page();
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

### أنظر أيضا

* class [TableCell](../)
* مساحة الاسم [Aspose.Note](../../tablecell/)
* المجسم [Aspose.Note](../../../)


