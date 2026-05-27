---
title: "RunIndex"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: 
type: docs
weight: 100
url: /ar/net/aspose.note/textstyle/runindex/
---
## TextStyle.RunIndex property

يحصل أو يضبط فهرس run index.

```csharp
public int RunIndex { get; set; }
```

### ملاحظات

فهرس run يحدد عدد الرمز الأخير في عقدة النص التي ستستخدم هذا النمط. يتم تعريف الرمز الأول على أنه التالي للرمز الأخير للنمط السابق في مجموعة الأنماط. يبدأ الفهرس من 1.

### أمثلة

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
* namespace [Aspose.Note](../../textstyle)
* assembly [Aspose.Note](../../../)

<!-- لا تقم بالتعديل: تم إنشاؤه بواسطة xmldocmd لـ Aspose.Note.dll -->
