---
title: "فئة ParagraphStyle"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "Aspose.Note.ParagraphStyle فئة. إعدادات نمط النص لاستخدامها إذا لم يكن هناك كائن TextStyle مطابق في مجموعة Styles أو إذا كان هذا الكائن لا يحدد الإعداد المطلوب"
type: docs
weight: 580
url: /ar/net/aspose.note/paragraphstyle/
---
## ParagraphStyle class

إعدادات نمط النص التي تُستخدم إذا لم يكن هناك كائن TextStyle مطابق في مجموعة Styles أو إذا لم يحدد هذا الكائن الإعداد المطلوب.

```csharp
public sealed class ParagraphStyle : Style, IEquatable<ParagraphStyle>
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [ParagraphStyle](paragraphstyle/)() | ينشئ مثلاً جديداً من الفئة `ParagraphStyle`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| static [Default](../../aspose.note/paragraphstyle/default/) { get; } | يحصل على الـ ParagraphStyle بالإعدادات الافتراضية. |
| [FontColor](../../aspose.note/style/fontcolor/) { get; set; } | يحصل أو يضبط لون الخط. |
| [FontName](../../aspose.note/style/fontname/) { get; set; } | يحصل أو يعيّن اسم الخط. |
| [FontSize](../../aspose.note/style/fontsize/) { get; set; } | يحصل أو يعيّن حجم الخط. |
| [FontStyle](../../aspose.note/style/fontstyle/) { get; } | يحصل على نمط الخط. |
| [Highlight](../../aspose.note/style/highlight/) { get; set; } | يحصل أو يضبط لون التظليل. |
| [IsBold](../../aspose.note/style/isbold/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان نمط النص غامقًا. |
| [IsItalic](../../aspose.note/style/isitalic/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان نمط النص مائلًا. |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان نمط النص مشطوبًا. |
| [IsSubscript](../../aspose.note/style/issubscript/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان نمط النص منخفضًا. |
| [IsSuperscript](../../aspose.note/style/issuperscript/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان نمط النص مرتفعًا. |
| [IsUnderline](../../aspose.note/style/isunderline/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان نمط النص تحته خط. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Equals](../../aspose.note/paragraphstyle/equals/#equals_1)(object) | يحدد ما إذا كان الكائن المحدد مساويًا للكائن الحالي. |
| [Equals](../../aspose.note/paragraphstyle/equals/#equals)(ParagraphStyle) | يحدد ما إذا كان الكائن المحدد مساويًا للكائن الحالي. |
| override [GetHashCode](../../aspose.note/paragraphstyle/gethashcode/)() | يعمل كدالة تجزئة للنوع. |

## أمثلة

دعنا نبرز عناوين الصفحة بين العناوين الأخرى بزيادة حجم الخط.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// حمّل المستند إلى Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// تكرار عبر عناوين الصفحة.
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

دعنا نبرز تغييرات النص الأخيرة عن طريق التظليل.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// حمّل المستند إلى Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// احصل على عقد RichText المعدلة الأسبوع الماضي.
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

التعامل مع تنسيق النص باستخدام نمط الفقرة.

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

* class [Style](../style/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


