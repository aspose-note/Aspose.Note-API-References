---
title: Class ParagraphStyle
second_title: Aspose.Note لمرجع NET API
description: Aspose.Note.ParagraphStyle فصل. يتم استخدام إعدادات نمط النص في حالة عدم وجود كائن TextStyle مطابق فيStyles مجموعة إما أن هذا الكائن لا يحدد الإعداد المطلوب.
type: docs
weight: 510
url: /ar/net/aspose.note/paragraphstyle/
---
## ParagraphStyle class

يتم استخدام إعدادات نمط النص في حالة عدم وجود كائن TextStyle مطابق فيStyles مجموعة إما أن هذا الكائن لا يحدد الإعداد المطلوب.

```csharp
public sealed class ParagraphStyle : Style, IEquatable<ParagraphStyle>
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [ParagraphStyle](paragraphstyle/)() | يقوم بتهيئة مثيل جديد لملف`ParagraphStyle` فئة . |

## الخصائص

| اسم | وصف |
| --- | --- |
| static [Default](../../aspose.note/paragraphstyle/default/) { get; } | الحصول على ParagraphStyle بالإعدادات الافتراضية. |
| [FontColor](../../aspose.note/style/fontcolor/) { get; set; } | الحصول على لون الخط أو تعيينه. |
| [FontName](../../aspose.note/style/fontname/) { get; set; } | الحصول على اسم الخط أو تحديده. |
| [FontSize](../../aspose.note/style/fontsize/) { get; set; } | الحصول على حجم الخط أو تحديده. |
| [FontStyle](../../aspose.note/style/fontstyle/) { get; } | يحصل على نمط الخط . |
| [Highlight](../../aspose.note/style/highlight/) { get; set; } | الحصول على لون التمييز أو تعيينه. |
| [IsBold](../../aspose.note/style/isbold/) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان نمط النص غامقًا . |
| [IsItalic](../../aspose.note/style/isitalic/) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان نمط النص مائلاً. |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough/) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان نمط النص يتوسطه خط أم لا. |
| [IsSubscript](../../aspose.note/style/issubscript/) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان نمط النص منخفضًا. |
| [IsSuperscript](../../aspose.note/style/issuperscript/) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان نمط النص مرتفعًا. |
| [IsUnderline](../../aspose.note/style/isunderline/) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان نمط النص تحته خط أم لا. |

## طُرق

| اسم | وصف |
| --- | --- |
| override [Equals](../../aspose.note/paragraphstyle/equals/#equals_1)(object) | تحديد ما إذا كان الكائن المحدد يساوي الكائن الحالي. |
| [Equals](../../aspose.note/paragraphstyle/equals/#equals)(ParagraphStyle) | تحديد ما إذا كان الكائن المحدد يساوي الكائن الحالي. |
| override [GetHashCode](../../aspose.note/paragraphstyle/gethashcode/)() | يعمل كدالة تجزئة للنوع. |

### أمثلة

دعنا نبرز عناوين الصفحة بين الرؤوس الأخرى عن طريق زيادة حجم الخط.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// قم بتحميل المستند في Aspose.
Document document = new Document(dataDir + "Aspose.one");

// تكرار من خلال عناوين الصفحة.
foreach (var title in document.Select(e => e.Title.TitleText))
{
    title.ParagraphStyle.FontSize = 24;
    title.ParagraphStyle.IsBold = true;

    foreach (var run in title.TextRuns)
    {
        run.Style.FontSize = 24;
        run.Style.IsBold = true;
    }
}

document.Save(Path.Combine(dataDir, "ChangePageTitleStyle.pdf"));
```

دعنا نؤكد على التغييرات الأخيرة في النص من خلال التمييز.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// قم بتحميل المستند في Aspose.
Document document = new Document(dataDir + "Aspose.one");

// Get RichText عُدلت الأسبوع الماضي.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // تعيين لون التظليل
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // تعيين لون التظليل
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

التلاعب بتنسيق النص باستخدام نمط الفقرة.

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = new ParagraphStyle() { FontName = "Courier New", FontSize = 20 } }
                .Append($"DefaultParagraphFontAndSize{Environment.NewLine}")
                .Append($"OnlyDefaultParagraphFont{Environment.NewLine}", new TextStyle() { FontSize = 14 })
                .Append("OnlyDefaultParagraphFontSize", new TextStyle() { FontName = "Verdana" });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetDefaultParagraphStyle.one"));
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

يوضح كيفية إدراج قائمة ذات تعداد نقطي جديد.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// إنشاء كائن من فئة المستند
Aspose.Note.Document doc = new Aspose.Note.Document();

// تهيئة كائن فئة الصفحة
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// تهيئة كائن فئة المخطط التفصيلي
Outline outline = new Outline(doc);

// تهيئة كائن فئة TextStyle وتعيين خصائص التنسيق
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// تهيئة كائنات فئة OutlineElement وتطبيق الرموز النقطية
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// تهيئة كائن فئة RichText وتطبيق نمط النص
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
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
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
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

* class [Style](../style/)
* مساحة الاسم [Aspose.Note](../../aspose.note/)
* المجسم [Aspose.Note](../../)


