---
title: Enum BinarizationMethod
second_title: Aspose.Note لمرجع NET API
description: Aspose.Note.Saving.BinarizationMethod تعداد. يحدد طريقة التحويل الثنائي للصورة.
type: docs
weight: 560
url: /ar/net/aspose.note.saving/binarizationmethod/
---
## BinarizationMethod enumeration

يحدد طريقة التحويل الثنائي للصورة.

```csharp
public enum BinarizationMethod
```

### قيم

| اسم | قيمة | وصف |
| --- | --- | --- |
| FixedThreshold | `0` | يتم تنفيذ التحويل الثنائي للصورة باستخدام حد ثابت محدد. |
| Otsu | `1` | يتم تنفيذ التحويل الثنائي للصورة بشكل تكيفي باستخدام طريقة Otsu لتقييم العتبة. |

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


