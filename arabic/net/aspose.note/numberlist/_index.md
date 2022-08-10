---
title: NumberList
second_title: Aspose.Note لمرجع NET API
description: يمثل القائمة المرقمة أو النقطية.
type: docs
weight: 420
url: /ar/net/aspose.note/numberlist/
---
## NumberList class

يمثل القائمة المرقمة أو النقطية.

```csharp
public class NumberList
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [NumberList](numberlist#constructor_1)(string, string, int) | يقوم بتهيئة مثيل جديد لملف[`NumberList`](../numberlist) class. يمثل هذا المثيل قائمة ذات تعداد نقطي. |
| [NumberList](numberlist#constructor)(string, NumberFormat, string, int) | يقوم بتهيئة مثيل جديد لملف[`NumberList`](../numberlist)class. يمثل هذا المثال قائمة مرقمة. |

## الخصائص

| اسم | وصف |
| --- | --- |
| [Font](../../aspose.note/numberlist/font) { get; set; } | الحصول على اسم الخط أو تحديده. |
| [FontColor](../../aspose.note/numberlist/fontcolor) { get; set; } | الحصول على لون الخط أو تعيينه. |
| [FontSize](../../aspose.note/numberlist/fontsize) { get; set; } | الحصول على حجم الخط أو تحديده. |
| [Format](../../aspose.note/numberlist/format) { get; set; } | الحصول على تنسيق عنوان السطر أو تحديده. بالنسبة للقوائم النقطية ، يمثل رمز التعداد النقطي. |
| [IsBold](../../aspose.note/numberlist/isbold) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان نمط النص غامقًا . |
| [IsItalic](../../aspose.note/numberlist/isitalic) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان نمط النص مائلاً. |
| [LastModifiedTime](../../aspose.note/numberlist/lastmodifiedtime) { get; set; } | الحصول على أو تعيين وقت آخر تعديل. |
| [NumberFormat](../../aspose.note/numberlist/numberformat) { get; set; } | الحصول على أو تحديد تنسيق الأرقام المستخدم لمجموعة من الكائنات المرقمة تلقائيًا. يجب أن يكون فارغًا للقوائم النقطية. |
| [Restart](../../aspose.note/numberlist/restart) { get; set; } | الحصول على أو تعيين القيمة الرقمية التي تتجاوز قيمة الرقم التلقائي لعنصر القائمة. |

## طُرق

| اسم | وصف |
| --- | --- |
| [Equals](../../aspose.note/numberlist/equals#equals)(NumberList) | تحديد ما إذا كان الكائن المحدد يساوي الكائن الحالي. |
| override [Equals](../../aspose.note/numberlist/equals#equals_1)(object) | تحديد ما إذا كان الكائن المحدد يساوي الكائن الحالي. |
| override [GetHashCode](../../aspose.note/numberlist/gethashcode)() | يعمل كدالة تجزئة للنوع. |
| [GetNumberedListHeader](../../aspose.note/numberlist/getnumberedlistheader)(int) | الحصول على رأس القائمة المرقمة . |

### أمثلة

يوضح كيفية استرداد المعلومات حول تنسيق القائمة.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// استرداد عقد مجموعة لعنصر المخطط التفصيلي
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// كرر خلال كل عقدة
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // استرداد اسم الخط
        Console.WriteLine("Font Name: " + list.Font);

        // استرداد طول الخط
        Console.WriteLine("Font Length: " + list.Font.Length);

        // استرداد حجم الخط
        Console.WriteLine("Font Size: " + list.FontSize);

        // استرداد لون الخط
        Console.WriteLine("Font Color: " + list.FontColor);

        // استرداد التنسيق
        Console.WriteLine("Font format: " + list.Format);

        // تحقق بخط عريض
        Console.WriteLine("Is bold: " + list.IsBold);

        // تحقق من الخط المائل
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

يوضح كيفية إدراج قائمة جديدة بالترقيم الصيني.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// تهيئة مستند OneNote
Aspose.Note.Document doc = new Aspose.Note.Document();

// تهيئة صفحة OneNote
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// تطبيق إعدادات نمط النص
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// يتم زيادة الأرقام الموجودة في نفس المخطط تلقائيًا.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

// ------------------------
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

// ------------------------
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// ------------------------
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// حفظ مستند OneNote
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

يوضح كيفية إدراج قائمة جديدة مع الترقيم.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// إنشاء كائن من فئة المستند
Document doc = new Document();

// تهيئة كائن فئة الصفحة
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// تهيئة كائن فئة المخطط التفصيلي
Outline outline = new Outline(doc);

// تهيئة كائن فئة TextStyle وتعيين خصائص التنسيق
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// تهيئة كائنات فئة OutlineElement وتطبيق الترقيم
// يتم زيادة الأرقام الموجودة في نفس المخطط تلقائيًا.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// أضف عناصر المخطط التفصيلي
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// إضافة عقدة المخطط التفصيلي
page.AppendChildLast(outline);

// إضافة عقدة الصفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

### أنظر أيضا

* مساحة الاسم [Aspose.Note](../../aspose.note)
* المجسم [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
