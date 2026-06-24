---
title: "الفئة TextStyle"
second_title: "مرجع API لـ Aspose.Note لـ .NET"
description: "الفئة Aspose.Note.TextStyle. تحدد نمط النص"
type: docs
weight: 1050
url: /ar/net/aspose.note/textstyle/
---
## TextStyle class

يحدد نمط النص.

```csharp
public sealed class TextStyle : Style
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [TextStyle](textstyle/)() | الباني الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| static [Default](../../aspose.note/textstyle/default/) { get; } | يحصل على النمط مع ثقافة "en-US". |
| static [DefaultMsOneNoteTitleDateStyle](../../aspose.note/textstyle/defaultmsonenotetitledatestyle/) { get; } | يحصل على النمط الافتراضي لتاريخ العنوان في MS OneNote. |
| static [DefaultMsOneNoteTitleTextStyle](../../aspose.note/textstyle/defaultmsonenotetitletextstyle/) { get; } | يحصل على النمط الافتراضي لنص العنوان في MS OneNote. |
| static [DefaultMsOneNoteTitleTimeStyle](../../aspose.note/textstyle/defaultmsonenotetitletimestyle/) { get; } | يحصل على النمط الافتراضي لوقت العنوان في MS OneNote. |
| [FontColor](../../aspose.note/style/fontcolor/) { get; set; } | يحصل أو يضبط لون الخط. |
| [FontName](../../aspose.note/style/fontname/) { get; set; } | يحصل أو يضبط اسم الخط. |
| [FontSize](../../aspose.note/style/fontsize/) { get; set; } | يحصل أو يضبط حجم الخط. |
| [FontStyle](../../aspose.note/style/fontstyle/) { get; } | يحصل على نمط الخط. |
| [Highlight](../../aspose.note/style/highlight/) { get; set; } | يحصل أو يضبط لون التظليل. |
| [HyperlinkAddress](../../aspose.note/textstyle/hyperlinkaddress/) { get; set; } | يحصل أو يضبط عنوان الارتباط التشعبي. ضبط هذه الخاصية يكفي لإنشاء ارتباط تشعبي. |
| [IsBold](../../aspose.note/style/isbold/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان نمط النص غامقًا. |
| [IsHidden](../../aspose.note/textstyle/ishidden/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان نمط النص مخفيًا. |
| [IsHyperlink](../../aspose.note/textstyle/ishyperlink/) { get; set; } | مهمل منذ 22.5. استخدم [HyperlinkAddress](../../aspose.note/textstyle/hyperlinkaddress/) بدلاً من ذلك. |
| [IsItalic](../../aspose.note/style/isitalic/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان نمط النص مائلًا. |
| [IsMathFormatting](../../aspose.note/textstyle/ismathformatting/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان نمط النص بتنسيق رياضي. |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان نمط النص مشطوبًا. |
| [IsSubscript](../../aspose.note/style/issubscript/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان نمط النص تحت السطر. |
| [IsSuperscript](../../aspose.note/style/issuperscript/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان نمط النص فوق السطر. |
| [IsUnderline](../../aspose.note/style/isunderline/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان نمط النص مسطرًا. |
| [Language](../../aspose.note/textstyle/language/) { get; set; } | يحصل أو يضبط لغة النص. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Equals](../../aspose.note/textstyle/equals/#equals_1)(object) | يحدد ما إذا كان الكائن المحدد يساوي الكائن الحالي. |
| [Equals](../../aspose.note/textstyle/equals/#equals)(TextStyle) | يحدد ما إذا كان الكائن المحدد يساوي الكائن الحالي. |
| override [GetHashCode](../../aspose.note/textstyle/gethashcode/)() | يعمل كدالة تجزئة (hash) لهذا النوع. |

## أمثلة

لنُبرز عناوين الصفحة بين باقي العناوين بزيادة حجم الخط.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// حمّل المستند إلى Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// تكرّر عبر عناوين الصفحة.
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

لنُبرز تغييرات النص الأخير عن طريق التظليل.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// حمّل المستند إلى Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// احصل على عقد RichText التي تم تعديلها الأسبوع الماضي.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // حدد لون التظليل
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // حدد لون التظليل
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

حدد لغة التدقيق للنص.

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

تلاعب بتنسيق النص باستخدام نمط الفقرة.

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

يعرض كيفية ربط ارتباط تشعبي بنص.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tasks();

// إنشاء كائن من الفئة Document
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
                                       HyperlinkAddress = "https://www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// إضافة عناصر المخطط
outline.AppendChildLast(outlineElem);

// تهيئة كائن فئة Title
Title title = new Title() { TitleText = titleText };

// تهيئة كائن الفئة Page
Page page = new Note.Page() { Title = title };

// إضافة عقدة المخطط
page.AppendChildLast(outline);

// إضافة عقدة الصفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

### انظر أيضًا

* class [Style](../style/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


