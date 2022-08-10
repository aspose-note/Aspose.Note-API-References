---
title: TextStyle
second_title: Aspose.Note لمرجع NET API
description: يحدد نمط النص .
type: docs
weight: 940
url: /ar/net/aspose.note/textstyle/
---
## TextStyle class

يحدد نمط النص .

```csharp
public sealed class TextStyle : Style
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [TextStyle](textstyle)() | Default_Constructor |

## الخصائص

| اسم | وصف |
| --- | --- |
| static [Default](../../aspose.note/textstyle/default) { get; } | الحصول على النمط الافتراضي لنص العنوان في MS OneNote . |
| static [DefaultMsOneNoteTitleDateStyle](../../aspose.note/textstyle/defaultmsonenotetitledatestyle) { get; } | الحصول على النمط الافتراضي لتاريخ العنوان في MS OneNote . |
| static [DefaultMsOneNoteTitleTextStyle](../../aspose.note/textstyle/defaultmsonenotetitletextstyle) { get; } | الحصول على النمط الافتراضي لنص العنوان في MS OneNote . |
| static [DefaultMsOneNoteTitleTimeStyle](../../aspose.note/textstyle/defaultmsonenotetitletimestyle) { get; } | الحصول على النمط الافتراضي لوقت العنوان في MS OneNote . |
| [FontColor](../../aspose.note/style/fontcolor) { get; set; } | الحصول على لون الخط أو تعيينه. |
| [FontName](../../aspose.note/style/fontname) { get; set; } | الحصول على اسم الخط أو تحديده. |
| [FontSize](../../aspose.note/style/fontsize) { get; set; } | الحصول على حجم الخط أو تحديده. |
| [FontStyle](../../aspose.note/style/fontstyle) { get; } | يحصل على نمط الخط . |
| [Highlight](../../aspose.note/style/highlight) { get; set; } | الحصول على لون التمييز أو تعيينه. |
| [HyperlinkAddress](../../aspose.note/textstyle/hyperlinkaddress) { get; set; } | الحصول على عنوان الارتباط التشعبي أو تعيينه. يجب تعيين إذا كانت قيمة[`IsHyperlink`](./ishyperlink) الخاصية صحيحة . |
| [IsBold](../../aspose.note/style/isbold) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان نمط النص غامقًا . |
| [IsHidden](../../aspose.note/textstyle/ishidden) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان نمط النص مخفيًا. |
| [IsHyperlink](../../aspose.note/textstyle/ishyperlink) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان نمط النص ارتباطًا تشعبيًا. |
| [IsItalic](../../aspose.note/style/isitalic) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان نمط النص مائلاً. |
| [IsMathFormatting](../../aspose.note/textstyle/ismathformatting) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان نمط النص بتنسيق رياضي. |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough) { get; set; } | الحصول على قيمة أو تعيينها للإشارة إلى ما إذا كان نمط النص يتوسطه خط أم لا. |
| [IsSubscript](../../aspose.note/style/issubscript) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان نمط النص منخفضًا. |
| [IsSuperscript](../../aspose.note/style/issuperscript) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان نمط النص مرتفعًا. |
| [IsUnderline](../../aspose.note/style/isunderline) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان نمط النص تحته خط أم لا. |
| [Language](../../aspose.note/textstyle/language) { get; set; } | الحصول على لغة النص أو تحديدها . |

## طُرق

| اسم | وصف |
| --- | --- |
| override [Equals](../../aspose.note/textstyle/equals#equals_1)(object) | تحديد ما إذا كان الكائن المحدد يساوي الكائن الحالي. |
| [Equals](../../aspose.note/textstyle/equals#equals)(TextStyle) | تحديد ما إذا كان الكائن المحدد يساوي الكائن الحالي. |
| override [GetHashCode](../../aspose.note/textstyle/gethashcode)() | يعمل كدالة تجزئة للنوع. |

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

تعيين لغة التدقيق للنص.

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = ParagraphStyle.Default };
text.Append("United States", new TextStyle() { Language = CultureInfo.GetCultureInfo("en-US") })
    .Append(" Germany", new TextStyle() { Language = CultureInfo.GetCultureInfo("de-DE") })
    .Append(" China", new TextStyle() { Language = CultureInfo.GetCultureInfo("zh-CN") });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetProofingLanguageForText.one"));
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

يوضح كيفية ربط ارتباط تشعبي بنص.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tasks();

// إنشاء كائن من فئة المستند
Document doc = new Document();

RichText titleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append("Title!");

Outline outline = new Outline()
                      {
                          MaxWidth = 200,
                          MaxHeight = 200,
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };

TextStyle textStyleRed = new TextStyle
                             {
                                 FontColor = Color.Red,
                                 FontName = "Arial",
                                 FontSize = 10,
                             };

TextStyle textStyleHyperlink = new TextStyle
                                   {
                                       IsHyperlink = true,
                                       HyperlinkAddress = "www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// أضف عناصر المخطط التفصيلي
outline.AppendChildLast(outlineElem);

// تهيئة كائن فئة العنوان
Title title = new Title() { TitleText = titleText };

// تهيئة كائن فئة الصفحة
Page page = new Note.Page() { Title = title };

// إضافة عقدة المخطط التفصيلي
page.AppendChildLast(outline);

// إضافة عقدة الصفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

### أنظر أيضا

* class [Style](../style)
* مساحة الاسم [Aspose.Note](../../aspose.note)
* المجسم [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
