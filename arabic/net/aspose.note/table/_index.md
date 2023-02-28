---
title: Class Table
second_title: Aspose.Note لمرجع NET API
description: Aspose.Note.Table فصل. يمثل جدول .
type: docs
weight: 900
url: /ar/net/aspose.note/table/
---
## Table class

يمثل جدول .

```csharp
public sealed class Table : CompositeNode<TableRow>, IOutlineElementChildNode, ITaggable
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [Table](table/#constructor)() | يقوم بتهيئة مثيل جديد لملف`Table` فئة . |

## الخصائص

| اسم | وصف |
| --- | --- |
| [Columns](../../aspose.note/table/columns/) { get; } | الحصول على أعمدة الجدول . |
| [Document](../../aspose.note/node/document/) { get; } | يحصل على وثيقة العقدة . |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IsBordersVisible](../../aspose.note/table/isbordersvisible/) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان حد الجدول مرئيًا. |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [LastModifiedTime](../../aspose.note/table/lastmodifiedtime/) { get; set; } | الحصول على أو تعيين وقت آخر تعديل. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | الحصول على العقدة التالية على نفس مستوى شجرة العقدة. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | يحصل على نوع العقدة . |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | يحصل على العقدة الأصلية . |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | الحصول على العقدة السابقة على نفس مستوى شجرة العقدة. |
| [Tags](../../aspose.note/table/tags/) { get; } | يحصل على قائمة بكافة علامات الفقرة . |

## طُرق

| اسم | وصف |
| --- | --- |
| override [Accept](../../aspose.note/table/accept/)(DocumentVisitor) | يقبل زائر العقدة . |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;TableRow&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params TableRow[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |

### أمثلة

يوضح كيفية الحصول على نص من صف كل جدول.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tables();

// قم بتحميل المستند في Aspose.
Document document = new Document(dataDir + "Sample1.one");

// احصل على قائمة بعقد الجدول
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // التكرار خلال صفوف الجدول
    foreach (TableRow row in table)
    {
        // استرداد النص
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // طباعة النص على شاشة الإخراج
        Console.WriteLine(text);
    }
}
```

يوضح كيفية الحصول على نص من جدول.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tables();

// قم بتحميل المستند في Aspose.
Document document = new Document(dataDir + "Sample1.one");

// احصل على قائمة بعقد الجدول
IList<Table> nodes = document.GetChildNodes<Table>();

// تعيين عدد الجدول
int tblCount = 0;

foreach (Table table in nodes)
{
    tblCount++;
    Console.WriteLine("table # " + tblCount);

    // استرداد النص
    string text = string.Join(Environment.NewLine, table.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

    // طباعة النص على شاشة الإخراج
    Console.WriteLine(text);
}
```

يوضح كيفية الحصول على نص من خلايا الجدول.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tables();

// قم بتحميل المستند في Aspose.
Document document = new Document(dataDir + "Sample1.one");

// احصل على قائمة بعقد الجدول
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // التكرار خلال صفوف الجدول
    foreach (TableRow row in table)
    {
        // احصل على قائمة بعقد TableCell
        // كرر خلال خلايا الجدول
        foreach (TableCell cell in row)
        {
            // استرداد النص
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // طباعة النص على شاشة الإخراج
            Console.WriteLine(text);
        }
    }
}
```

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

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* class [TableRow](../tablerow/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [ITaggable](../itaggable/)
* مساحة الاسم [Aspose.Note](../../aspose.note/)
* المجسم [Aspose.Note](../../)


