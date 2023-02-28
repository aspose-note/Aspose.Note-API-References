---
title: TableColumn.LockedWidth
second_title: Aspose.Note لمرجع NET API
description: TableColumn ملكية. الحصول على أو تعيين قيمة تشير إلى ما إذا كان عرض عمود الجدول مغلقًا ولا يتم تغيير حجمه تلقائيًا ليلائم محتوى الجدول. افتراضيًا  لا يتم تأمين عرض العمود.
type: docs
weight: 20
url: /ar/net/aspose.note/tablecolumn/lockedwidth/
---
## TableColumn.LockedWidth property

الحصول على أو تعيين قيمة تشير إلى ما إذا كان عرض عمود الجدول مغلقًا ولا يتم تغيير حجمه تلقائيًا ليلائم محتوى الجدول. افتراضيًا ، لا يتم تأمين عرض العمود.

```csharp
public bool LockedWidth { get; set; }
```

### أمثلة

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

### أنظر أيضا

* class [TableColumn](../)
* مساحة الاسم [Aspose.Note](../../tablecolumn/)
* المجسم [Aspose.Note](../../../)


