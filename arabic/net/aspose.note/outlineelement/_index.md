---
title: "الفئة OutlineElement"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "الفئة Aspose.Note.OutlineElement. تمثل عنصر OutlineElement."
type: docs
weight: 530
url: /ar/net/aspose.note/outlineelement/
---
## OutlineElement class

يمثل عنصر مخطط.

```csharp
public sealed class OutlineElement : IndentatedNode<IOutlineElementChildNode>, IOutlineChildNode, 
    IOutlineElementChildNode
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [OutlineElement](outlineelement/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AuthorMostRecent](../../aspose.note/outlineelement/authormostrecent/) { get; } | يحصل على أحدث مؤلف لعنصر مخطط. |
| [AuthorOriginal](../../aspose.note/outlineelement/authororiginal/) { get; } | يحصل على المؤلف الأصلي لعنصر مخطط. |
| [CreationTime](../../aspose.note/outlineelement/creationtime/) { get; set; } | يحصل أو يعيّن وقت الإنشاء. |
| [Document](../../aspose.note/node/document/) { get; } | يحصل على مستند العقدة. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IndentPosition](../../aspose.note/indentatednode-1/indentposition/) { get; set; } |  |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [LastModifiedTime](../../aspose.note/outlineelement/lastmodifiedtime/) { get; set; } | يحصل أو يعيّن وقت آخر تعديل. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | يحصل على العقدة التالية في نفس مستوى شجرة العقد. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | يحصل على نوع العقدة. |
| [NumberList](../../aspose.note/outlineelement/numberlist/) { get; set; } | الحصول على أو تعيين النمط لرأس القائمة المرقمة. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | يحصل على العقدة الأصلية. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | يحصل على العقدة السابقة في نفس مستوى شجرة العقد. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Accept](../../aspose.note/outlineelement/accept/)(DocumentVisitor) | يقبل زائر العقدة. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;IOutlineElementChildNode&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params IOutlineElementChildNode[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |

## أمثلة

يعرض كيفية إضافة صورة جديدة مع علامة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tags();

// إنشاء كائن من فئة Document
Document doc = new Document();

// تهيئة كائن فئة Page
Page page = new Page();

// تهيئة كائن فئة Outline
Outline outline = new Outline();

// تهيئة كائن فئة OutlineElement
OutlineElement outlineElem = new OutlineElement();

// تحميل صورة.
Image image = new Image(dataDir + "icon.jpg");

// إدراج صورة في عقدة المستند.
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// إضافة عقدة عنصر المخطط
outline.AppendChildLast(outlineElem);

// إضافة عقدة المخطط
page.AppendChildLast(outline);

// إضافة عقدة صفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote.
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
```

يوضح كيفية استرجاع معلومات حول تنسيق القائمة.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// استرجاع مجموعة العقد لعنصر المخطط.
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// تكرار عبر كل عقدة
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // استرجاع اسم الخط
        Console.WriteLine("Font Name: " + list.Font);

        // استرجاع طول الخط
        Console.WriteLine("Font Length: " + list.Font.Length);

        // استرجاع حجم الخط
        Console.WriteLine("Font Size: " + list.FontSize);

        // استرجاع لون الخط
        Console.WriteLine("Font Color: " + list.FontColor);

        // استرجاع التنسيق
        Console.WriteLine("Font format: " + list.Format);

        // التحقق من الغامق
        Console.WriteLine("Is bold: " + list.IsBold);

        // التحقق من المائل
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

يعرض كيفية إدراج قائمة جديدة بترقيم صيني.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// تهيئة مستند OneNote.
Document doc = new Document();

// تهيئة صفحة OneNote.
Page page = new Page();
Outline outline = new Outline();

// تطبيق إعدادات نمط النص.
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// الأرقام في نفس المخطط تُزاد تلقائيًا.
OutlineElement outlineElem1 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText() { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

//------------------------
OutlineElement outlineElem2 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText() { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

//------------------------
OutlineElement outlineElem3 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText() { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

//------------------------
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// حفظ مستند OneNote.
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

يعرض كيفية إدراج قائمة نقطية جديدة.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// إنشاء كائن من فئة Document
Document doc = new Document();

// تهيئة كائن فئة Page
Page page = new Page();

// تهيئة كائن فئة Outline
Outline outline = new Outline();

// تهيئة كائن الفئة TextStyle وتعيين خصائص التنسيق
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// تهيئة كائنات الفئة OutlineElement وتطبيق النقاط
OutlineElement outlineElem1 = new OutlineElement() { NumberList = new NumberList("*", "Arial", 10) };

// تهيئة كائن الفئة RichText وتطبيق نمط النص
RichText text1 = new RichText() { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement() { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(  ) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement() { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText() { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// إضافة عناصر المخطط
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// إضافة عقدة المخطط
page.AppendChildLast(outline);
// إضافة عقدة الصفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote.
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

يعرض كيفية إدراج قائمة جديدة مع الترقيم.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// إنشاء كائن من فئة Document
Document doc = new Document();

// تهيئة كائن فئة Page
Page page = new Page();

// تهيئة كائن فئة Outline
Outline outline = new Outline();

// تهيئة كائن الفئة TextStyle وتعيين خصائص التنسيق
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// تهيئة كائنات الفئة OutlineElement وتطبيق الترقيم.
// الأرقام في نفس المخطط تُزاد تلقائيًا.
OutlineElement outlineElem1 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText() { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText() { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText() { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// إضافة عناصر المخطط
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// إضافة عقدة المخطط
page.AppendChildLast(outline);

// إضافة عقدة الصفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote.
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

### انظر أيضًا

* class [IndentatedNode&lt;T&gt;](../indentatednode-1/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [IOutlineChildNode](../ioutlinechildnode/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


