---
title: Class ImageSaveOptions
second_title: Aspose.Note لمرجع NET API
description: Aspose.Note.Saving.ImageSaveOptions فصل. يسمح بتحديد خيارات إضافية عند عرض صفحات المستند على الصور.
type: docs
weight: 720
url: /ar/net/aspose.note.saving/imagesaveoptions/
---
## ImageSaveOptions class

يسمح بتحديد خيارات إضافية عند عرض صفحات المستند على الصور.

```csharp
public class ImageSaveOptions : SaveOptions
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions/)(SaveFormat) | يقوم بتهيئة مثيل جديد لملف`ImageSaveOptions` فئة . |

## الخصائص

| اسم | وصف |
| --- | --- |
| [BinarizationOptions](../../aspose.note.saving/imagesaveoptions/binarizationoptions/) { get; set; } | الحصول على أو تعيين خيارات لترميز الصورة بالترميز الثنائي . |
| [ColorMode](../../aspose.note.saving/imagesaveoptions/colormode/) { get; set; } | يحصل أو يحدد[`ColorMode`](./colormode/) للصورة الناتجة. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | الحصول على أو تعيين إعدادات الخط لاستخدامها أثناء الحفظ |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | الحصول على أو تحديد عدد الصفحات المراد حفظها. افتراضيا هوMaxValue مما يعني أنه سيتم تقديم جميع صفحات المستند. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | الحصول على أو تحديد فهرس الصفحة الأولى للحفظ. بشكل افتراضي هو 0. |
| [Quality](../../aspose.note.saving/imagesaveoptions/quality/) { get; set; } | الحصول على أو تعيين قيمة تحدد جودة الصورة المحفوظة. يتم تمرير هذه القيمة إلى برنامج الترميز مثل System.Drawing.Imaging.Encoder.Quality parameter. |
| [Resolution](../../aspose.note.saving/imagesaveoptions/resolution/) { get; set; } | الحصول على أو تعيين دقة الصور التي تم إنشاؤها ، بالنقاط في البوصة . |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | يحصل على التنسيق الذي تم حفظ المستند به. |
| [TiffCompression](../../aspose.note.saving/imagesaveoptions/tiffcompression/) { get; set; } | الحصول على أو تحديد نوع الضغط المطلوب استخدامه عند حفظ الصور المُنشأة بتنسيق TIFF. |

### أمثلة

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

يوضح كيفية ضبط جودة الصورة عند حفظ المستند كصورة بتنسيق JPEG.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// احفظ المستند.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
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

يوضح كيفية ضبط دقة الصورة عند حفظ المستند كصورة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// احفظ المستند.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
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

يوضح كيفية حفظ دفتر الملاحظات كصورة بخيارات محددة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

// تحميل دفتر ملاحظات OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// حفظ دفتر الملاحظات
notebook.Save(dataDir, notebookSaveOptions);
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

يوضح كيفية حفظ دفتر الملاحظات المسطح كصورة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

// تحميل دفتر ملاحظات OneNote
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// حفظ دفتر الملاحظات
notebook.Save(dataDir, notebookSaveOptions);
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

يوضح كيفية حفظ مستند بتنسيق png.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "Aspose.one");

// تهيئة كائن ImageSaveOptions 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // تعيين فهرس الصفحة
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// احفظ المستند بصيغة PNG.
oneFile.Save(dataDir, opts);
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

* class [SaveOptions](../saveoptions/)
* مساحة الاسم [Aspose.Note.Saving](../../aspose.note.saving/)
* المجسم [Aspose.Note](../../)


