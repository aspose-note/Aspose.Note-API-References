---
title: Save
second_title: Aspose.Note لمرجع NET API
description: يحفظ مستند OneNote في ملف.
type: docs
weight: 140
url: /ar/net/aspose.note/document/save/
---
## Save(string) {#save_3}

يحفظ مستند OneNote في ملف.

```csharp
public void Save(string fileName)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| fileName | String | الاسم الكامل للملف. إذا كان هناك ملف بالاسم الكامل المحدد موجودًا بالفعل ، فسيتم استبدال الملف الحالي. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | هيكل الوثيقة ينتهك المواصفات. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | تنسيق الحفظ المطلوب غير مدعوم. |

### أمثلة

يوضح كيفية حفظ مستند.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

### أنظر أيضا

* class [Document](../../document)
* مساحة الاسم [Aspose.Note](../../document)
* المجسم [Aspose.Note](../../../)

---

## Save(Stream) {#save}

يحفظ مستند OneNote في دفق.

```csharp
public void Save(Stream stream)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| stream | Stream | System.IO.Stream حيث سيتم حفظ المستند. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | هيكل الوثيقة ينتهك المواصفات. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | تنسيق الحفظ المطلوب غير مدعوم. |

### أنظر أيضا

* class [Document](../../document)
* مساحة الاسم [Aspose.Note](../../document)
* المجسم [Aspose.Note](../../../)

---

## Save(string, SaveFormat) {#save_4}

يحفظ مستند OneNote في ملف بالتنسيق المحدد.

```csharp
public void Save(string fileName, SaveFormat format)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| fileName | String | الاسم الكامل للملف. إذا كان هناك ملف بالاسم الكامل المحدد موجودًا بالفعل ، فسيتم استبدال الملف الحالي. |
| format | SaveFormat | التنسيق المراد حفظ المستند به. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | هيكل الوثيقة ينتهك المواصفات. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | تنسيق الحفظ المطلوب غير مدعوم. |

### أمثلة

يوضح كيفية حفظ مستند باستخدام تعداد SaveFormat.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

يوضح كيفية حفظ مستند بتنسيق gif.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// احفظ المستند بصيغة gif.
oneFile.Save(dataDir, SaveFormat.Gif);
```

### أنظر أيضا

* enum [SaveFormat](../../saveformat)
* class [Document](../../document)
* مساحة الاسم [Aspose.Note](../../document)
* المجسم [Aspose.Note](../../../)

---

## Save(Stream, SaveFormat) {#save_1}

يحفظ مستند OneNote في دفق بالتنسيق المحدد.

```csharp
public void Save(Stream stream, SaveFormat format)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| stream | Stream | System.IO.Stream حيث سيتم حفظ المستند. |
| format | SaveFormat | التنسيق المراد حفظ المستند به. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | هيكل الوثيقة ينتهك المواصفات. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | تنسيق الحفظ المطلوب غير مدعوم. |

### أمثلة

يوضح كيفية حفظ مستند بتنسيق pdf باستخدام الإعدادات الافتراضية.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "Aspose.one");

// احفظ المستند بصيغة PDF
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

يوضح كيفية حفظ مستند في دفق.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// قم بإرجاع موضع الدفق إلى الصفر بحيث يكون جاهزًا للقارئ التالي.
dstStream.Seek(0, SeekOrigin.Begin);
```

### أنظر أيضا

* enum [SaveFormat](../../saveformat)
* class [Document](../../document)
* مساحة الاسم [Aspose.Note](../../document)
* المجسم [Aspose.Note](../../../)

---

## Save(string, SaveOptions) {#save_5}

يحفظ مستند OneNote في ملف باستخدام خيارات الحفظ المحددة.

```csharp
public void Save(string fileName, SaveOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| fileName | String | الاسم الكامل للملف. إذا كان هناك ملف بالاسم الكامل المحدد موجودًا بالفعل ، فسيتم استبدال الملف الحالي. |
| options | SaveOptions | يحدد الخيارات كيفية حفظ المستند في ملف. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | هيكل الوثيقة ينتهك المواصفات. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | تنسيق الحفظ المطلوب غير مدعوم. |

### أمثلة

يوضح كيفية حفظ مستند باستخدام OneSaveOptions.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

يوضح كيفية حفظ مستند كصورة بتنسيق Jpeg باستخدام SaveFormat.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToJpegImageUsingSaveFormat_out.jpg";

// احفظ المستند.
oneFile.Save(dataDir, SaveFormat.Jpeg);
```

يوضح كيفية حفظ مستند كصورة بتنسيق Bmp باستخدام ImageSaveOptions.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBmpImageUsingImageSaveOptions_out.bmp";

// احفظ المستند.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Bmp));
```

يوضح كيفية حفظ مستند كصورة ذات تدرج رمادي.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveAsGrayscaleImage_out.png";

// احفظ المستند بصيغة gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.GrayScale
                          });
```

يوضح كيفية حفظ مستند كصورة بتنسيق Tiff باستخدام ضغط PackBits.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingPackBitsCompression.tiff");

// احفظ المستند.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.PackBits
                      });
```

يوضح كيفية حفظ مستند كصورة بتنسيق Tiff باستخدام ضغط Jpeg.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// احفظ المستند.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

يوضح كيفية حفظ مستند كصورة بتنسيق Tiff باستخدام ضغط الفاكس CCITT Group 3.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
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

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "Aspose.one");

// تهيئة كائن PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // تعيين فهرس الصفحة للصفحة الأولى ليتم حفظها
                              PageIndex = 0,

                              // تعيين عدد الصفحات
                              PageCount = 1,
                          };

// احفظ المستند بصيغة PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

يوضح كيفية حفظ مستند بتنسيق pdf باستخدام إعدادات محددة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document doc = new Document(dataDir + "Aspose.one");

// تهيئة كائن PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // استخدم ضغط Jpeg
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // جودة ضغط JPEG
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

يوضح كيفية حفظ مستند كصورة ثنائية باستخدام طريقة Otsu.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
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

يوضح كيفية حفظ مستند كصورة ثنائية باستخدام عتبة ثابتة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
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

### أنظر أيضا

* class [SaveOptions](../../../aspose.note.saving/saveoptions)
* class [Document](../../document)
* مساحة الاسم [Aspose.Note](../../document)
* المجسم [Aspose.Note](../../../)

---

## Save(Stream, SaveOptions) {#save_2}

يحفظ مستند OneNote في دفق باستخدام خيارات الحفظ المحددة.

```csharp
public void Save(Stream stream, SaveOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| stream | Stream | System.IO.Stream حيث سيتم حفظ المستند. |
| options | SaveOptions | يحدد الخيارات كيفية حفظ المستند في الدفق. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | هيكل الوثيقة ينتهك المواصفات. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | تنسيق الحفظ المطلوب غير مدعوم. |

### أمثلة

يوضح كيفية حفظ مستند بتنسيق pdf باستخدام الخط الافتراضي المحدد.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// احفظ المستند بصيغة PDF
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

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// احفظ المستند بصيغة PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

يوضح كيفية حفظ مستند بتنسيق pdf باستخدام الخط الافتراضي من التدفق.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// احفظ المستند بصيغة PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### أنظر أيضا

* class [SaveOptions](../../../aspose.note.saving/saveoptions)
* class [Document](../../document)
* مساحة الاسم [Aspose.Note](../../document)
* المجسم [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
