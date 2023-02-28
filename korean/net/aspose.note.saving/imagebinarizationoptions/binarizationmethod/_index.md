---
title: ImageBinarizationOptions.BinarizationMethod
second_title: .NET API 참조용 Aspose.Note
description: ImageBinarizationOptions 재산. 이진화 방법을 가져오거나 설정합니다. 기본값은FixedThreshold .
type: docs
weight: 20
url: /ko/net/aspose.note.saving/imagebinarizationoptions/binarizationmethod/
---
## ImageBinarizationOptions.BinarizationMethod property

이진화 방법을 가져오거나 설정합니다. 기본값은FixedThreshold .

```csharp
public BinarizationMethod BinarizationMethod { get; set; }
```

### 예

Otsu의 방법을 사용하여 문서를 바이너리 이미지로 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingOtsuMethod_out.png";

// 문서를 gif로 저장합니다.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                        {
                            ColorMode = ColorMode.BlackAndWhite,
                            BinarizationOptions = new ImageBinarizationOptions()
                                                  {
                                                      BinarizationMethod = BinarizationMethod.Otsu,
                                                  }
                        });
```

고정 임계값을 사용하여 문서를 바이너리 이미지로 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingFixedThreshold_out.png";

// 문서를 gif로 저장합니다.
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

### 또한보십시오

* enum [BinarizationMethod](../../binarizationmethod/)
* class [ImageBinarizationOptions](../)
* 네임스페이스 [Aspose.Note.Saving](../../imagebinarizationoptions/)
* 집회 [Aspose.Note](../../../)


