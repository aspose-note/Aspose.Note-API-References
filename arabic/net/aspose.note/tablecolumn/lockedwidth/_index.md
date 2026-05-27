---
title: "TableColumn.LockedWidth"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية TableColumn. يحصل أو يحدد قيمة تشير إلى ما إذا كان عرض عمود الجدول مقفلًا ولا يتم تغيير حجمه تلقائيًا ليتناسب مع محتوى الجدول. بشكل افتراضي، عرض العمود غير مقفل"
type: docs
weight: 20
url: /ar/net/aspose.note/tablecolumn/lockedwidth/
---
## TableColumn.LockedWidth property

يحصل أو يضبط قيمة تشير إلى ما إذا كان عمود الجدول يمتلك عرضًا مقفلًا ولا يعيد حجمه تلقائيًا لتناسب محتوى الجدول. بشكل افتراضي، عرض العمود غير مقفل.

```csharp
public bool LockedWidth { get; set; }
```

## أمثلة

يوضح كيفية إنشاء جدول بعمود مقفل.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tables();

// إنشاء كائن من فئة Document
Document doc = new Document();

// تهيئة كائن فئة Page
Page page = new Page();

// تهيئة كائن فئة TableRow
TableRow row1 = new TableRow();

// تهيئة كائن فئة TableCell وتعيين محتوى النص
TableCell cell11 = new TableCell();
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText("Small text"));
row1.AppendChildLast(cell11);

// تهيئة كائن فئة TableRow
TableRow row2 = new TableRow();

// تهيئة كائن فئة TableCell وتعيين محتوى النص
TableCell cell21 = new TableCell();
cell21.AppendChildLast(InsertTable.GetOutlineElementWithText("Long   text    with    several   words and    spaces."));
row2.AppendChildLast(cell21);

// تهيئة كائن فئة Table
Table table = new Table()
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70, LockedWidth = true } }
              };

// إضافة صفوف
table.AppendChildLast(row1);
table.AppendChildLast(row2);

Outline outline = new Outline();
OutlineElement outlineElem = new OutlineElement();

// إضافة عقدة جدول
outlineElem.AppendChildLast(table);

// إضافة عقدة عنصر المخطط
outline.AppendChildLast(outlineElem);

// إضافة عقدة المخطط
page.AppendChildLast(outline);

// إضافة عقدة صفحة
doc.AppendChildLast(page);
dataDir = dataDir + "CreateTableWithLockedColumns_out.one";
doc.Save(dataDir);
```

### انظر أيضًا

* class [TableColumn](../)
* namespace [Aspose.Note](../../tablecolumn/)
* assembly [Aspose.Note](../../../)


