---
title: "الفئة TableRow"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "Aspose.Note.TableRow فئة. يمثل صف جدول"
type: docs
weight: 1010
url: /ar/net/aspose.note/tablerow/
---
## TableRow class

يمثل صف جدول.

```csharp
public sealed class TableRow : CompositeNode<TableCell>
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [TableRow](tablerow/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | يحصل على مستند العقدة. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [LastModifiedTime](../../aspose.note/tablerow/lastmodifiedtime/) { get; set; } | يحصل أو يعيّن وقت آخر تعديل. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | يحصل على العقدة التالية في نفس مستوى شجرة العقد. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | يحصل على نوع العقدة. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | يحصل على العقدة الأصلية. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | يحصل على العقدة السابقة في نفس مستوى شجرة العقد. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Accept](../../aspose.note/tablerow/accept/)(DocumentVisitor) | يقبل زائر العقدة. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;TableCell&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params TableCell[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |

## أمثلة

يوضح كيفية الحصول على النص من كل صف في الجدول.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tables();

// حمّل المستند إلى Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// احصل على قائمة بعقد الجدول
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // التكرار عبر صفوف الجدول
    foreach (TableRow row in table)
    {
        // استرجاع النص
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // طباعة النص على شاشة الإخراج
        Console.WriteLine(text);
    }
}
```

يوضح كيفية الحصول على النص من خلايا الجدول.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tables();

// حمّل المستند إلى Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// احصل على قائمة بعقد الجدول
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // التكرار عبر صفوف الجدول
    foreach (TableRow row in table)
    {
        // احصل على قائمة بعقد TableCell
        // التكرار عبر خلايا الجدول
        foreach (TableCell cell in row)
        {
            // استرجاع النص
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // طباعة النص على شاشة الإخراج
            Console.WriteLine(text);
        }
    }
}
```

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

يعرض كيفية إضافة جدول جديد مع العلامة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tags();

// إنشاء كائن من فئة Document
Document doc = new Document();

// تهيئة كائن فئة Page
Page page = new Page();

// تهيئة كائن فئة TableRow
TableRow row = new TableRow();

// تهيئة كائن فئة TableCell
TableCell cell = new TableCell();

// إدراج محتوى الخلية
cell.AppendChildLast(InsertTable.GetOutlineElementWithText("Single cell."));

// إضافة خلية إلى عقدة الصف
row.AppendChildLast(cell);

// تهيئة عقدة الجدول
Table table = new Table()
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70 } }
              };

// إدراج عقدة الصف في الجدول
table.AppendChildLast(row);

// إضافة علامة إلى عقدة الجدول هذه
table.Tags.Add(NoteTag.CreateQuestionMark());

Outline outline = new Outline();
OutlineElement outlineElem = new OutlineElement();

// إضافة عقدة جدول
outlineElem.AppendChildLast(table);

// إضافة عناصر المخطط
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// حفظ مستند OneNote.
dataDir = dataDir + "AddTableNodeWithTag_out.one";
doc.Save(dataDir);
```

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

يوضح كيفية إنشاء جدول جديد.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tables();

// إنشاء كائن من فئة Document
Document doc = new Document();

// تهيئة كائن فئة Page
Page page = new Page();

// تهيئة كائن فئة TableRow
TableRow row1 = new TableRow();

// تهيئة كائنات فئة TableCell
TableCell cell11 = new TableCell();
TableCell cell12 = new TableCell();
TableCell cell13 = new TableCell();

// إلحاق عناصر المخطط في خلية الجدول
cell11.AppendChildLast(GetOutlineElementWithText("cell_1.1"));
cell12.AppendChildLast(GetOutlineElementWithText("cell_1.2"));
cell13.AppendChildLast(GetOutlineElementWithText("cell_1.3"));

// خلايا الجدول إلى صفوف
row1.AppendChildLast(cell11);
row1.AppendChildLast(cell12);
row1.AppendChildLast(cell13);

// تهيئة كائن فئة TableRow
TableRow row2 = new TableRow();

// تهيئة كائنات فئة TableCell
TableCell cell21 = new TableCell();
TableCell cell22 = new TableCell();
TableCell cell23 = new TableCell();

// إلحاق عناصر المخطط في خلية الجدول
cell21.AppendChildLast(GetOutlineElementWithText("cell_2.1"));
cell22.AppendChildLast(GetOutlineElementWithText("cell_2.2"));
cell23.AppendChildLast(GetOutlineElementWithText("cell_2.3"));

// إلحاق خلايا الجدول إلى صفوف
row2.AppendChildLast(cell21);
row2.AppendChildLast(cell22);
row2.AppendChildLast(cell23);

// تهيئة كائن فئة Table وتعيين عرض الأعمدة
Table table = new Table()
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 200 }, new TableColumn { Width = 200 }, new TableColumn { Width = 200 } }
              };

// إلحاق صفوف الجدول بالجدول
table.AppendChildLast(row1);
table.AppendChildLast(row2);

// تهيئة كائن Outline
Outline outline = new Outline();

// تهيئة كائن OutlineElement
OutlineElement outlineElem = new OutlineElement();

// إضافة الجدول إلى عقدة عنصر المخطط
outlineElem.AppendChildLast(table);

// إضافة عنصر المخطط إلى المخطط
outline.AppendChildLast(outlineElem);

// إضافة المخطط إلى عقدة الصفحة
page.AppendChildLast(outline);

// إضافة الصفحة إلى عقدة المستند
doc.AppendChildLast(page);
dataDir = dataDir + "InsertTable_out.one";
doc.Save(dataDir);
```

### انظر أيضًا

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* class [TableCell](../tablecell/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


