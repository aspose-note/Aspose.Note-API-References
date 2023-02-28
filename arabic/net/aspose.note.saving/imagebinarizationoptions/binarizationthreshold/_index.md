---
title: ImageBinarizationOptions.BinarizationThreshold
second_title: Aspose.Note لمرجع NET API
description: ImageBinarizationOptions ملكية. الحصول على أو تعيين قيمة حد لطريقة ترميز العتبة الثنائية الثابتة . القيمة الافتراضية هي 128.
type: docs
weight: 30
url: /ar/net/aspose.note.saving/imagebinarizationoptions/binarizationthreshold/
---
## ImageBinarizationOptions.BinarizationThreshold property

الحصول على أو تعيين قيمة حد لطريقة ترميز العتبة الثنائية الثابتة . القيمة الافتراضية هي 128.

```csharp
public byte BinarizationThreshold { get; set; }
```

### أمثلة

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

* class [ImageBinarizationOptions](../)
* مساحة الاسم [Aspose.Note.Saving](../../imagebinarizationoptions/)
* المجسم [Aspose.Note](../../../)


