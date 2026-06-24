---
title: "ImageSaveOptions.BinarizationOptions"
second_title: "مرجع API لـ Aspose.Note لـ .NET"
description: "خاصية ImageSaveOptions. تحصل أو تعيين خيارات لتصنيف الصور إلى ثنائي"
type: docs
weight: 20
url: /ar/net/aspose.note.saving/imagesaveoptions/binarizationoptions/
---
## ImageSaveOptions.BinarizationOptions property

يحصل أو يعيّن خيارات تحويل الصورة إلى ثنائية.

```csharp
public ImageBinarizationOptions BinarizationOptions { get; set; }
```

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

* class [ImageBinarizationOptions](../../imagebinarizationoptions/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Note.Saving](../../imagesaveoptions/)
* assembly [Aspose.Note](../../../)


