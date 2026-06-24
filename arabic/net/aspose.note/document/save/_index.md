---
title: "Document.Save"
second_title: "مرجع API لـ Aspose.Note لـ .NET"
description: "طريقة Document. يحفظ مستند OneNote إلى ملف"
type: docs
weight: 140
url: /ar/net/aspose.note/document/save/
---
## Save(string) {#save_3}

يحفظ مستند OneNote إلى ملف.

```csharp
public void Save(string fileName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | String | الاسم الكامل للملف. إذا كان هناك ملف بالاسم الكامل المحدد موجودًا بالفعل، يتم استبدال الملف الموجود. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | هيكل المستند ينتهك المواصفات. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | تنسيق الحفظ المطلوب غير مدعوم. |

## أمثلة

يوضح كيفية حفظ مستند.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

### انظر أيضًا

* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Save(Stream) {#save}

يحفظ مستند OneNote إلى تدفق.

```csharp
public void Save(Stream stream)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream | تدفق System.IO.Stream حيث سيتم حفظ المستند. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | هيكل المستند ينتهك المواصفات. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | تنسيق الحفظ المطلوب غير مدعوم. |

### انظر أيضًا

* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Save(string, SaveFormat) {#save_4}

يحفظ مستند OneNote إلى ملف بالتنسيق المحدد.

```csharp
public void Save(string fileName, SaveFormat format)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | String | الاسم الكامل للملف. إذا كان هناك ملف بالاسم الكامل المحدد موجودًا بالفعل، يتم استبدال الملف الموجود. |
| تنسيق | SaveFormat | التنسيق الذي سيتم حفظ المستند به. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | هيكل المستند ينتهك المواصفات. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | تنسيق الحفظ المطلوب غير مدعوم. |

## أمثلة

يعرض كيفية حفظ مستند باستخدام تعداد SaveFormat.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

يعرض كيفية حفظ مستند بصيغة gif.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// احفظ المستند بصيغة gif.
oneFile.Save(dataDir, SaveFormat.Gif);
```

### انظر أيضًا

* enum [SaveFormat](../../saveformat/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Save(Stream, SaveFormat) {#save_1}

يحفظ مستند OneNote إلى تدفق بالتنسيق المحدد.

```csharp
public void Save(Stream stream, SaveFormat format)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream | تدفق System.IO.Stream حيث سيتم حفظ المستند. |
| تنسيق | SaveFormat | التنسيق الذي سيتم حفظ المستند به. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | هيكل المستند ينتهك المواصفات. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | تنسيق الحفظ المطلوب غير مدعوم. |

## أمثلة

يوضح كيفية تحويل مستند OneNote إلى صيغة HTML.

```csharp
var dataDir = RunExamples.GetDataDir_Conversion_Html();

var oneFilePath = Path.Combine(dataDir, "sample.one");
var htmlFilePath = Path.Combine(dataDir, "output.html");

// تحويل OneNote إلى HTML
var doc = new Document(oneFilePath);
doc.Save(htmlFilePath, SaveFormat.Html);
```

يعرض كيفية حفظ مستند بصيغة pdf باستخدام الإعدادات الافتراضية.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// احفظ المستند كملف PDF
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

يعرض كيفية حفظ مستند إلى تدفق.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// أعد موضع التدفق إلى الصفر حتى يكون جاهزًا للقارئ التالي.
dstStream.Seek(0, SeekOrigin.Begin);
```

يوضح كيفية تحويل مستند OneNote إلى صيغة Markdown.

```csharp
var dataDir = RunExamples.GetDataDir_Conversion_Markdown();

var oneFilePath = Path.Combine(dataDir, "sample.one");
var mdFilePath = Path.Combine(dataDir, "output.md");
var htmlFilePath = Path.Combine(dataDir, "temp.html");

// تحويل OneNote إلى HTML
var document = new Document(oneFilePath);
document.Save(htmlFilePath, SaveFormat.Html);

// تحويل HTML إلى Markdown
Converter.ConvertHTML(htmlFilePath, new MarkdownSaveOptions(), mdFilePath);

Console.WriteLine("\nOneNote document converted to Markdown successfully.");
```

يوضح كيفية تطبيق نمط السمة الداكنة على مستند.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Text();

// حمّل المستند إلى Aspose.Note.
Document doc = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in doc)
{
    page.BackgroundColor = Color.Black;
}

foreach (var node in doc.GetChildNodes<RichText>())
{
    var c = node.ParagraphStyle.FontColor;
    if (c.IsEmpty || Math.Abs(c.R - Color.Black.R) + Math.Abs(c.G - Color.Black.G) + Math.Abs(c.B - Color.Black.B) <= 30)
    {
        node.ParagraphStyle.FontColor = Color.White;
    }
}

doc.Save(Path.Combine(dataDir, "AsposeDarkTheme.pdf"));
```

### انظر أيضًا

* enum [SaveFormat](../../saveformat/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Save(string, SaveOptions) {#save_5}

يحفظ مستند OneNote إلى ملف باستخدام خيارات الحفظ المحددة.

```csharp
public void Save(string fileName, SaveOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | String | الاسم الكامل للملف. إذا كان هناك ملف بالاسم الكامل المحدد موجودًا بالفعل، يتم استبدال الملف الموجود. |
| خيارات | SaveOptions | يحدد الخيارات التي يتم حفظ المستند بها في الملف. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | هيكل المستند ينتهك المواصفات. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | تنسيق الحفظ المطلوب غير مدعوم. |

## أمثلة

يعرض كيفية حفظ مستند باستخدام OneSaveOptions.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

يوضح كيفية حفظ المستند كصورة بتنسيق Jpeg باستخدام SaveFormat.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToJpegImageUsingSaveFormat_out.jpg";

// احفظ المستند.
oneFile.Save(dataDir, SaveFormat.Jpeg);
```

يوضح كيفية حفظ المستند كصورة بتنسيق Bmp باستخدام ImageSaveOptions.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBmpImageUsingImageSaveOptions_out.bmp";

// احفظ المستند.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Bmp));
```

يعرض كيفية حفظ مستند بتنسيق Pdf مع تخطيط صفحة Letter.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// احفظ المستند.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

يعرض كيفية حفظ مستند بتنسيق Pdf مع تخطيط صفحة A4 دون حد للارتفاع.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// احفظ المستند.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
```

يوضح كيفية حفظ المستند كصورة بتدرج الرمادي.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveAsGrayscaleImage_out.png";

// احفظ المستند بصيغة gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.GrayScale
                          });
```

يوضح كيفية حفظ المستند كصورة بتنسيق Tiff باستخدام ضغط PackBits.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingPackBitsCompression.tiff");

// احفظ المستند.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.PackBits
                      });
```

يوضح كيفية حفظ المستند كصورة بتنسيق Tiff باستخدام ضغط Jpeg.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// احفظ المستند.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

يوضح كيفية حفظ المستند كصورة بتنسيق Tiff باستخدام ضغط الفاكس CCITT Group 3.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingCcitt3Compression.tiff");

// احفظ المستند.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          ColorMode = ColorMode.BlackAndWhite,
                          TiffCompression = TiffCompression.Ccitt3
                      });
```

يوضح كيفية حفظ مستند بتنسيق pdf.

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

يوضح كيفية حفظ مستند بتنسيق pdf باستخدام إعدادات محددة.

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

يوضح كيفية حفظ المستند كصورة ثنائية باستخدام طريقة Otsu.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingOtsuMethod_out.png";

// احفظ المستند بصيغة gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                        {
                            ColorMode = ColorMode.BlackAndWhite,
                            BinarizationOptions = new ImageBinarizationOptions()
                                                  {
                                                      BinarizationMethod = BinarizationMethod.Otsu,
                                                  }
                        });
```

يوضح كيفية حفظ المستند كصورة ثنائية باستخدام عتبة ثابتة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingFixedThreshold_out.png";

// احفظ المستند بصيغة gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.BlackAndWhite,
                              BinarizationOptions = new ImageBinarizationOptions()
                                                        {
                                                            BinarizationMethod = BinarizationMethod.FixedThreshold,
                                                            BinarizationThreshold = 123
                                                        }
                          });
```

### انظر أيضًا

* class [SaveOptions](../../../aspose.note.saving/saveoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Save(Stream, SaveOptions) {#save_2}

يحفظ مستند OneNote إلى تدفق باستخدام خيارات الحفظ المحددة.

```csharp
public void Save(Stream stream, SaveOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream | تدفق System.IO.Stream حيث سيتم حفظ المستند. |
| خيارات | SaveOptions | يحدد الخيارات التي يتم بها حفظ المستند في الدفق. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | هيكل المستند ينتهك المواصفات. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | تنسيق الحفظ المطلوب غير مدعوم. |

## أمثلة

يوضح كيفية حفظ مستند بتنسيق pdf باستخدام الخط الافتراضي المحدد.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// احفظ المستند كملف PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

يوضح كيفية حفظ مستند بتنسيق pdf باستخدام الخط الافتراضي من ملف.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// احفظ المستند كملف PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

يوضح كيفية حفظ مستند بتنسيق pdf باستخدام الخط الافتراضي من تدفق.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// احفظ المستند كملف PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### انظر أيضًا

* class [SaveOptions](../../../aspose.note.saving/saveoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)


