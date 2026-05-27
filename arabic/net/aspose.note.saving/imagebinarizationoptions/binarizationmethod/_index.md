---
title: "ImageBinarizationOptions.BinarizationMethod"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية ImageBinarizationOptions. تحصل أو تعين طريقة التحويل الثنائي. القيمة الافتراضية هي FixedThreshold"
type: docs
weight: 20
url: /ar/net/aspose.note.saving/imagebinarizationoptions/binarizationmethod/
---
## ImageBinarizationOptions.BinarizationMethod property

يحصل أو يضبط طريقة التحويل إلى ثنائي. القيمة الافتراضية هي FixedThreshold.

```csharp
public BinarizationMethod BinarizationMethod { get; set; }
```

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

* enum [BinarizationMethod](../../binarizationmethod/)
* class [ImageBinarizationOptions](../)
* namespace [Aspose.Note.Saving](../../imagebinarizationoptions/)
* assembly [Aspose.Note](../../../)


