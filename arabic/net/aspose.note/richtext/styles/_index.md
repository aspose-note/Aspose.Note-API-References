---
title: "الأنماط"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: 
type: docs
weight: 80
url: /ar/net/aspose.note/richtext/styles/
---
## RichText.Styles property

يحصل على الأنماط.

```csharp
public IList<TextStyle> Styles { get; }
```

### أمثلة

يظهر كيفية تغيير النمط لنص.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// حمّل المستند إلى Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// احصل على عقدة RichText معينة
RichText richText = document.GetChildNodes<RichText>().First();

foreach (TextStyle style in richText.Styles)
{
    // تعيين لون الخط
    style.FontColor = Color.Yellow;

    // تعيين لون التظليل
    style.Highlight = Color.Blue;

    // تعيين حجم الخط
    style.FontSize = 20;
}
```

لنقم بتنسيق الجدول لتحسين الإدراك. اجعل صف الرأس غامقًا ومائلًا، وميّز كل صف زوجي باستخدام اللون LightGray.

```csharp
string dataDir = RunExamples.GetDataDir_Tables();

// حمّل المستند إلى Aspose.Note.
Document document = new Document(dataDir + "ChangeTableStyleIn.one");

// احصل على قائمة بعقد الجدول
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    SetRowStyle(table.First(), Color.DarkGray, true, true);

    // تمييز الصف الأول بعد الرأس.
    var flag = false;
    foreach (var row in table.Skip(1))
    {
        SetRowStyle(row, flag ? Color.LightGray : Color.Empty, false, false);

        flag = !flag;
    }
}

document.Save(Path.Combine(dataDir, "ChangeTableStyleOut.one"));
```

تعيين لغة التدقيق لنص.

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { Text = "United States Germany China", ParagraphStyle = ParagraphStyle.Default };
text.Styles.Add(new TextStyle()
                    {
                        Language = CultureInfo.GetCultureInfo("en-US"),
                        RunIndex = 13
                    });
text.Styles.Add(new TextStyle()
                    {
                        Language = CultureInfo.GetCultureInfo("de-DE"),
                        RunIndex = 21
                    });
text.Styles.Add(new TextStyle()
                    {
                        Language = CultureInfo.GetCultureInfo("zh-CN"),
                        RunIndex = text.Text.Length
                    });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetProofingLanguageForText.one"));
```

يظهر كيفية ربط ارتباط تشعبي بنص.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tasks();

// إنشاء كائن من فئة Document
Document doc = new Document();

RichText titleText = new RichText()
                     {
                         Text = "Title!",
                         ParagraphStyle = ParagraphStyle.Default
                     };

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

                             // سيتم تطبيق هذا النمط على الأحرف من 0 إلى 7.
                             RunIndex = 8 
                         };

TextStyle textStyleHyperlink = new TextStyle
                              {
                                  // سيتم تطبيق هذا النمط على الأحرف من 8 إلى 16.
                                  RunIndex = 17,
                                  HyperlinkAddress = "https://www.google.com"
                              };

RichText text = new RichText()
                {
                    Text = "This is hyperlink. This text is not a hyperlink.",
                    ParagraphStyle = ParagraphStyle.Default,
                    Styles = { textStyleRed, textStyleHyperlink }
                };

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// إضافة عناصر المخطط
outline.AppendChildLast(outlineElem);

// تهيئة كائن فئة Title
Title title = new Title() { TitleText = titleText };

// تهيئة كائن فئة Page
Aspose.Note.Page page = new Aspose.Note.Page(doc) { Title = title };

// إضافة عقدة المخطط
page.AppendChildLast(outline);

// إضافة عقدة الصفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote.
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

### انظر أيضًا

* class [TextStyle](../../textstyle)
* class [RichText](../../richtext)
* namespace [Aspose.Note](../../richtext)
* assembly [Aspose.Note](../../../)

<!-- لا تقم بالتعديل: تم إنشاؤه بواسطة xmldocmd لـ Aspose.Note.dll -->
