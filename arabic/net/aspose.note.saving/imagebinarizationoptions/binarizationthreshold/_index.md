---
title: "ImageBinarizationOptions.BinarizationThreshold"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية ImageBinarizationOptions. تحصل أو تعين قيمة العتبة لطريقة التحويل الثنائي بالعتبة الثابتة. القيمة الافتراضية هي 128"
type: docs
weight: 30
url: /ar/net/aspose.note.saving/imagebinarizationoptions/binarizationthreshold/
---
## ImageBinarizationOptions.BinarizationThreshold property

يحصل أو يضبط قيمة العتبة لطريقة التحويل إلى ثنائي ذات العتبة الثابتة. القيمة الافتراضية هي 128.

```csharp
public byte BinarizationThreshold { get; set; }
```

## أمثلة

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

* class [ImageBinarizationOptions](../)
* namespace [Aspose.Note.Saving](../../imagebinarizationoptions/)
* assembly [Aspose.Note](../../../)


