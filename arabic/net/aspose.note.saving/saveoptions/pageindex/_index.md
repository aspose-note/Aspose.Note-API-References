---
title: "SaveOptions.PageIndex"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية SaveOptions. تحصل أو تعين فهرس الصفحة الأولى للحفظ. القيمة الافتراضية هي 0"
type: docs
weight: 30
url: /ar/net/aspose.note.saving/saveoptions/pageindex/
---
## SaveOptions.PageIndex property

يحصل أو يضبط فهرس الصفحة الأولى التي سيتم حفظها. القيمة الافتراضية هي 0.

```csharp
public int PageIndex { get; set; }
```

## أمثلة

يظهر كيفية حفظ مستند بتنسيق png.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// تهيئة كائن ImageSaveOptions 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // تعيين فهرس الصفحة
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// حفظ المستند كـ PNG.
oneFile.Save(dataDir, opts);
```

يظهر كيفية حفظ مستند بتنسيق pdf.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// تهيئة كائن PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // تعيين فهرس الصفحة الأولى التي سيتم حفظها
                              PageIndex = 0,

                              // تعيين عدد الصفحات
                              PageCount = 1,
                          };

// احفظ المستند كملف PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

يظهر كيفية حفظ مستند بتنسيق pdf باستخدام إعدادات محددة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// تهيئة كائن PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // استخدام ضغط Jpeg
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // جودة ضغط JPEG
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

يوضح كيفية إنشاء مستند وحفظه بتنسيق html لنطاق محدد من الصفحات.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// تهيئة مستند OneNote.
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// النمط الافتراضي لجميع النصوص في المستند.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// حفظ بتنسيق HTML
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

يعرض كيفية إنشاء مستند بنص غني منسق.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// إنشاء كائن من فئة Document
Document doc = new Document();

// تهيئة كائن فئة Page
Page page = new Page();

// تهيئة كائن فئة Title
Title title = new Title();

// تهيئة كائن الفئة TextStyle وتعيين خصائص التنسيق
ParagraphStyle defaultTextStyle = new ParagraphStyle
                                      {
                                          FontColor = Color.Black,
                                          FontName = "Arial",
                                          FontSize = 10
                                      };

RichText titleText = new RichText() { ParagraphStyle = defaultTextStyle }.Append("Title!");
Outline outline = new Outline()
                      {
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };
OutlineElement outlineElem = new OutlineElement();

TextStyle textStyleForHelloWord = new TextStyle
                                      {
                                          FontColor = Color.Red,
                                          FontName = "Arial",
                                          FontSize = 10,
                                      };

TextStyle textStyleForOneNoteWord = new TextStyle
                                        {
                                            FontColor = Color.Green,
                                            FontName = "Calibri",
                                            FontSize = 10,
                                            IsItalic = true,
                                        };

TextStyle textStyleForTextWord = new TextStyle
                                     {
                                         FontColor = Color.Blue,
                                         FontName = "Arial",
                                         FontSize = 15,
                                         IsBold = true,
                                         IsItalic = true,
                                     };

RichText text = new RichText() { ParagraphStyle = defaultTextStyle }
                    .Append("Hello", textStyleForHelloWord)
                    .Append(" OneNote", textStyleForOneNoteWord)
                    .Append(" text", textStyleForTextWord)
                    .Append("!", TextStyle.Default);

title.TitleText = titleText;

// تعيين عنوان الصفحة
page.Title = title;

// إضافة عقدة RichText
outlineElem.AppendChildLast(text);

// إضافة عقدة OutlineElement
outline.AppendChildLast(outlineElem);

// إضافة عقدة المخطط
page.AppendChildLast(outline);

// إضافة عقدة الصفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote.
dataDir = dataDir + "CreateDocWithFormattedRichText_out.one";
doc.Save(dataDir);
```

### انظر أيضًا

* class [SaveOptions](../)
* namespace [Aspose.Note.Saving](../../saveoptions/)
* assembly [Aspose.Note](../../../)


