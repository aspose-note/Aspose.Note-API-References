---
title: Enum BinarizationMethod
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.Saving.BinarizationMethod 열거형. 이미지의 이진화 방법을 지정합니다.
type: docs
weight: 560
url: /ko/net/aspose.note.saving/binarizationmethod/
---
## BinarizationMethod enumeration

이미지의 이진화 방법을 지정합니다.

```csharp
public enum BinarizationMethod
```

### 가치

| 이름 | 값 | 설명 |
| --- | --- | --- |
| FixedThreshold | `0` | 지정된 고정 임계값을 사용하여 이미지의 이진화가 수행됩니다. |
| Otsu | `1` | 이미지의 이진화는 임계값을 평가하기 위해 Otsu의 방법을 사용하여 적응적으로 수행됩니다. |

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

* 네임스페이스 [Aspose.Note.Saving](../../aspose.note.saving/)
* 집회 [Aspose.Note](../../)


