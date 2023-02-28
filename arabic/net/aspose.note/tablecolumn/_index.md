---
title: Class TableColumn
second_title: Aspose.Note لمرجع NET API
description: Aspose.Note.TableColumn فصل. يمثل عمود جدول .
type: docs
weight: 920
url: /ar/net/aspose.note/tablecolumn/
---
## TableColumn class

يمثل عمود جدول .

```csharp
public sealed class TableColumn
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [TableColumn](tablecolumn/)() | Default_Constructor |

## الخصائص

| اسم | وصف |
| --- | --- |
| [LockedWidth](../../aspose.note/tablecolumn/lockedwidth/) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان عرض عمود الجدول مغلقًا ولا يتم تغيير حجمه تلقائيًا ليلائم محتوى الجدول. افتراضيًا ، لا يتم تأمين عرض العمود. |
| [Width](../../aspose.note/tablecolumn/width/) { get; set; } | الحصول على العرض أو تحديده . |

### أمثلة

يوضح كيفية تعيين لون الخلفية لخلية.

```csharp
// إنشاء كائن من فئة المستند
Document doc = new Document();

// تهيئة كائن فئة TableCell وتعيين محتوى النص
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
cell11.BackgroundColor = Color.Coral;

// تهيئة كائن فئة TableRow
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

// تهيئة كائن فئة الصفحة
Page page = new Page(doc);
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

يوضح كيفية إضافة جدول جديد بعلامة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tags();

// إنشاء كائن من فئة المستند
Document doc = new Document();

// تهيئة كائن فئة الصفحة
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// تهيئة كائن فئة TableRow
TableRow row = new TableRow(doc);

// تهيئة كائن فئة TableCell
TableCell cell = new TableCell(doc);

// أدخل محتوى الخلية
cell.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Single cell."));

// أضف خلية إلى عقدة صف
row.AppendChildLast(cell);

// تهيئة عقدة الجدول
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70 } }
              };

// أدخل عقدة صف في الجدول
table.AppendChildLast(row);

// أضف علامة إلى عقدة الجدول هذه
table.Tags.Add(NoteTag.CreateQuestionMark());

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// إضافة عقدة الجدول
outlineElem.AppendChildLast(table);

// أضف عناصر المخطط التفصيلي
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// حفظ مستند OneNote
dataDir = dataDir + "AddTableNodeWithTag_out.one";
doc.Save(dataDir);
```

يوضح كيفية إنشاء جدول بعمود مؤمن.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tables();

// إنشاء كائن من فئة المستند
Document doc = new Document();

// تهيئة كائن فئة الصفحة
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// تهيئة كائن فئة TableRow
TableRow row1 = new TableRow(doc);

// تهيئة كائن فئة TableCell وتعيين محتوى النص
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
row1.AppendChildLast(cell11);

// تهيئة كائن فئة TableRow
TableRow row2 = new TableRow(doc);

// تهيئة كائن فئة TableCell وتعيين محتوى النص
TableCell cell21 = new TableCell(doc);
cell21.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Long   text    with    several   words and    spaces."));
row2.AppendChildLast(cell21);

// تهيئة كائن فئة الجدول
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70, LockedWidth = true } }
              };

// إضافة صفوف
table.AppendChildLast(row1);
table.AppendChildLast(row2);

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// إضافة عقدة الجدول
outlineElem.AppendChildLast(table);

// إضافة عقدة عنصر المخطط التفصيلي
outline.AppendChildLast(outlineElem);

// إضافة عقدة المخطط التفصيلي
page.AppendChildLast(outline);

// إضافة عقدة الصفحة
doc.AppendChildLast(page);
dataDir = dataDir + "CreateTableWithLockedColumns_out.one";
doc.Save(dataDir);
```

يوضح كيفية إنشاء جدول جديد.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tables();

// إنشاء كائن من فئة المستند
Document doc = new Document();

// تهيئة كائن فئة الصفحة
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// تهيئة كائن فئة TableRow
TableRow row1 = new TableRow(doc);

// تهيئة كائنات فئة TableCell
TableCell cell11 = new TableCell(doc);
TableCell cell12 = new TableCell(doc);
TableCell cell13 = new TableCell(doc);

// إلحاق عناصر المخطط التفصيلي في خلية الجدول
cell11.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.1"));
cell12.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.2"));
cell13.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.3"));

// خلايا الجدول إلى صفوف
row1.AppendChildLast(cell11);
row1.AppendChildLast(cell12);
row1.AppendChildLast(cell13);

// تهيئة كائن فئة TableRow
TableRow row2 = new TableRow(doc);

// تهيئة كائنات فئة TableCell
TableCell cell21 = new TableCell(doc);
TableCell cell22 = new TableCell(doc);
TableCell cell23 = new TableCell(doc);

// إلحاق عناصر المخطط التفصيلي في خلية الجدول
cell21.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.1"));
cell22.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.2"));
cell23.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.3"));

// إلحاق خلايا الجدول بالصفوف
row2.AppendChildLast(cell21);
row2.AppendChildLast(cell22);
row2.AppendChildLast(cell23);

// تهيئة كائن فئة الجدول وتعيين عرض العمود
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 200 }, new TableColumn { Width = 200 }, new TableColumn { Width = 200 } }
              };

// إلحاق صفوف الجدول بالجدول
table.AppendChildLast(row1);
table.AppendChildLast(row2);

// تهيئة كائن المخطط التفصيلي
Outline outline = new Outline(doc);

// تهيئة كائن OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// إضافة جدول إلى مخطط عقدة العنصر
outlineElem.AppendChildLast(table);

// إضافة عنصر المخطط التفصيلي إلى مخطط تفصيلي
outline.AppendChildLast(outlineElem);

// إضافة مخطط إلى عقدة الصفحة
page.AppendChildLast(outline);

// إضافة صفحة إلى عقدة الوثيقة
doc.AppendChildLast(page);
dataDir = dataDir + "InsertTable_out.one";
doc.Save(dataDir);
```

### أنظر أيضا

* مساحة الاسم [Aspose.Note](../../aspose.note/)
* المجسم [Aspose.Note](../../)


