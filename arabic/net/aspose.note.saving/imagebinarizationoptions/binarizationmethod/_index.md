---
title: ImageBinarizationOptions.BinarizationMethod
second_title: Aspose.Note لمرجع NET API
description: ImageBinarizationOptions ملكية. الحصول على طريقة الترميز الثنائي أو تعيينها . القيمة الافتراضية هيFixedThreshold .
type: docs
weight: 20
url: /ar/net/aspose.note.saving/imagebinarizationoptions/binarizationmethod/
---
## ImageBinarizationOptions.BinarizationMethod property

الحصول على طريقة الترميز الثنائي أو تعيينها . القيمة الافتراضية هيFixedThreshold .

```csharp
public BinarizationMethod BinarizationMethod { get; set; }
```

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

* enum [BinarizationMethod](../../binarizationmethod/)
* class [ImageBinarizationOptions](../)
* مساحة الاسم [Aspose.Note.Saving](../../imagebinarizationoptions/)
* المجسم [Aspose.Note](../../../)


