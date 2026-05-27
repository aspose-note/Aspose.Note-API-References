---
title: "تعداد BinarizationMethod"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "تعداد Aspose.Note.Saving.BinarizationMethod. يحدد طريقة التثنث لصورة"
type: docs
weight: 640
url: /ar/net/aspose.note.saving/binarizationmethod/
---
## BinarizationMethod enumeration

يحدد طريقة التثنائي للصورة.

```csharp
public enum BinarizationMethod
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| FixedThreshold | `0` | يتم تنفيذ تثنث الصورة باستخدام العتبة الثابتة المحددة. |
| Otsu | `1` | يتم تنفيذ تثنث الصورة بشكل تكيفي باستخدام طريقة أوتسو لتقييم العتبة. |

## أمثلة

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


