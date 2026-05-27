---
title: "الفئة NumberList"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "الفئة Aspose.Note.NumberList. تمثل القائمة المرقمة أو القائمة ذات الرموز النقطية"
type: docs
weight: 510
url: /ar/net/aspose.note/numberlist/
---
## NumberList class

يمثل القائمة المرقمة أو ذات النقاط.

```csharp
public class NumberList
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [NumberList](numberlist/#constructor_1)(string, string, int) | يُنشئ مثيلاً جديداً من الفئة `NumberList`. هذا المثيل يمثل قائمة ذات رموز نقطية. |
| [NumberList](numberlist/#constructor)(string, NumberFormat, string, int) | يُنشئ مثيلاً جديداً من الفئة `NumberList`. هذا المثيل يمثل قائمة مرقمة. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Font](../../aspose.note/numberlist/font/) { get; set; } | يحصل أو يعيّن اسم الخط. |
| [FontColor](../../aspose.note/numberlist/fontcolor/) { get; set; } | يحصل أو يضبط لون الخط. |
| [FontSize](../../aspose.note/numberlist/fontsize/) { get; set; } | يحصل أو يعيّن حجم الخط. |
| [Format](../../aspose.note/numberlist/format/) { get; set; } | يحصل أو يعيّن تنسيق رأس السطر. بالنسبة للقوائم ذات الرموز النقطية يمثل رمزًا نقطيًا. |
| [IsBold](../../aspose.note/numberlist/isbold/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان نمط النص غامقًا. |
| [IsItalic](../../aspose.note/numberlist/isitalic/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان نمط النص مائلًا. |
| [LastModifiedTime](../../aspose.note/numberlist/lastmodifiedtime/) { get; set; } | يحصل أو يعيّن وقت آخر تعديل. |
| [NumberFormat](../../aspose.note/numberlist/numberformat/) { get; set; } | يحصل أو يعيّن تنسيق الرقم المستخدم لمجموعة من الكائنات المرقمة تلقائيًا. يجب أن يكون فارغًا للقوائم ذات الرموز النقطية. |
| [Restart](../../aspose.note/numberlist/restart/) { get; set; } | يحصل أو يعيّن القيمة الرقمية التي تتجاوز القيمة العددية التلقائية لعنصر القائمة. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Equals](../../aspose.note/numberlist/equals/#equals)(NumberList) | يحدد ما إذا كان الكائن المحدد مساويًا للكائن الحالي. |
| override [Equals](../../aspose.note/numberlist/equals/#equals_1)(object) | يحدد ما إذا كان الكائن المحدد مساويًا للكائن الحالي. |
| override [GetHashCode](../../aspose.note/numberlist/gethashcode/)() | يعمل كدالة تجزئة للنوع. |
| [GetNumberedListHeader](../../aspose.note/numberlist/getnumberedlistheader/)(int) | يحصل على رأس القائمة المرقمة. |

## أمثلة

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

* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


