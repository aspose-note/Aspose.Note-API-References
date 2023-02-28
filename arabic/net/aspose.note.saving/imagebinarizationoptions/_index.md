---
title: Class ImageBinarizationOptions
second_title: Aspose.Note لمرجع NET API
description: Aspose.Note.Saving.ImageBinarizationOptions فصل. خيارات لترميز الصورة بالترميز .
type: docs
weight: 710
url: /ar/net/aspose.note.saving/imagebinarizationoptions/
---
## ImageBinarizationOptions class

خيارات لترميز الصورة بالترميز .

```csharp
public class ImageBinarizationOptions
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [ImageBinarizationOptions](imagebinarizationoptions/)() | Default_Constructor |

## الخصائص

| اسم | وصف |
| --- | --- |
| [BinarizationMethod](../../aspose.note.saving/imagebinarizationoptions/binarizationmethod/) { get; set; } | الحصول على طريقة الترميز الثنائي أو تعيينها . القيمة الافتراضية هيFixedThreshold . |
| [BinarizationThreshold](../../aspose.note.saving/imagebinarizationoptions/binarizationthreshold/) { get; set; } | الحصول على أو تعيين قيمة حد لطريقة ترميز العتبة الثنائية الثابتة . القيمة الافتراضية هي 128. |

### أمثلة

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

* مساحة الاسم [Aspose.Note.Saving](../../aspose.note.saving/)
* المجسم [Aspose.Note](../../)


