---
title: "التعداد ColorMode"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "التعداد Aspose.Note.Saving.ColorMode. وضع اللون للصورة"
type: docs
weight: 650
url: /ar/net/aspose.note.saving/colormode/
---
## ColorMode enumeration

وضع اللون للصورة.

```csharp
public enum ColorMode
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Normal | `0` | صورة ملونة بالكامل |
| GrayScale | `1` | صورة بتدرج الرمادي |
| BlackAndWhite | `2` | صورة ثنائية: تُستخدم فقط الألوان الأسود والأبيض |

## أمثلة

يظهر كيفية حفظ المستند كصورة بتدرج الرمادي.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveAsGrayscaleImage_out.png";

// احفظ المستند كـ gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.GrayScale
                          });
```

يظهر كيفية حفظ المستند كصورة بتنسيق Tiff باستخدام ضغط CCITT Group 3 fax.

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

يظهر كيفية حفظ المستند كصورة ثنائية باستخدام طريقة Otsu.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingOtsuMethod_out.png";

// احفظ المستند كـ gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                        {
                            ColorMode = ColorMode.BlackAndWhite,
                            BinarizationOptions = new ImageBinarizationOptions()
                                                  {
                                                      BinarizationMethod = BinarizationMethod.Otsu,
                                                  }
                        });
```

يظهر كيفية حفظ المستند كصورة ثنائية باستخدام عتبة ثابتة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingFixedThreshold_out.png";

// احفظ المستند كـ gif.
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

* namespace [Aspose.Note.Saving](../../aspose.note.saving/)
* assembly [Aspose.Note](../../)


