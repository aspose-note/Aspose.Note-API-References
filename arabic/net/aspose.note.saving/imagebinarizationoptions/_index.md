---
title: "الفئة ImageBinarizationOptions"
second_title: "مرجع API لـ Aspose.Note لـ .NET"
description: "Aspose.Note.Saving.ImageBinarizationOptions class. خيارات لتصنيف الصور إلى ثنائية"
type: docs
weight: 790
url: /ar/net/aspose.note.saving/imagebinarizationoptions/
---
## ImageBinarizationOptions class

خيارات ثنائية الصورة.

```csharp
public class ImageBinarizationOptions
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [ImageBinarizationOptions](imagebinarizationoptions/)() | الباني الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BinarizationMethod](../../aspose.note.saving/imagebinarizationoptions/binarizationmethod/) { get; set; } | يحصل أو يضبط طريقة التحويل إلى ثنائي. القيمة الافتراضية هي FixedThreshold. |
| [BinarizationThreshold](../../aspose.note.saving/imagebinarizationoptions/binarizationthreshold/) { get; set; } | يحصل أو يضبط قيمة العتبة لطريقة التحويل إلى ثنائي ذات العتبة الثابتة. القيمة الافتراضية هي 128. |

## أمثلة

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

* namespace [Aspose.Note.Saving](../../aspose.note.saving/)
* assembly [Aspose.Note](../../)


