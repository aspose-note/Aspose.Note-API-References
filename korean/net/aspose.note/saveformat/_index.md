---
title: Enum SaveFormat
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.SaveFormat 열거형. 문서가 저장되는 형식을 나타냅니다.
type: docs
weight: 540
url: /ko/net/aspose.note/saveformat/
---
## SaveFormat enumeration

문서가 저장되는 형식을 나타냅니다.

```csharp
public enum SaveFormat
```

### 가치

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Png | `1` | 출력이 PNG 파일임을 지정합니다. |
| Bmp | `2` | 출력이 BMP 파일임을 지정합니다. |
| Jpeg | `3` | 출력이 JPEG 파일임을 지정합니다. |
| Gif | `4` | 출력이 GIF 파일임을 지정합니다. |
| Tiff | `5` | 출력이 TIFF 파일임을 지정합니다. |
| Pdf | `6` | 출력이 PDF 파일임을 지정합니다. |
| One | `7` | 출력이 OneNote 파일임을 지정합니다. |
| Html | `8` | 출력이 HTML 파일임을 지정합니다. |

### 예

SaveFormat 열거형을 사용하여 문서를 저장하는 방법을 보여줍니다.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

기본 설정을 사용하여 PDF 형식으로 문서를 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "Aspose.one");

// 문서를 PDF로 저장
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

SaveFormat을 사용하여 문서를 Jpeg 형식의 이미지로 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToJpegImageUsingSaveFormat_out.jpg";

// 문서를 저장합니다.
oneFile.Save(dataDir, SaveFormat.Jpeg);
```

문서를 gif 형식으로 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// 문서를 gif로 저장합니다.
oneFile.Save(dataDir, SaveFormat.Gif);
```

문서를 JPEG 형식의 이미지로 저장할 때 이미지 품질을 설정하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// 문서를 저장합니다.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

ImageSaveOptions를 사용하여 문서를 Bmp 형식의 이미지로 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBmpImageUsingImageSaveOptions_out.bmp";

// 문서를 저장합니다.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Bmp));
```

문서를 이미지로 저장할 때 이미지 해상도를 설정하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// 문서를 저장합니다.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

문서를 그레이스케일 이미지로 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveAsGrayscaleImage_out.png";

// 문서를 gif로 저장합니다.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.GrayScale
                          });
```

PackBits 압축을 사용하여 문서를 Tiff 형식의 이미지로 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingPackBitsCompression.tiff");

// 문서를 저장합니다.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.PackBits
                      });
```

Jpeg 압축을 사용하여 문서를 Tiff 형식의 이미지로 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// 문서를 저장합니다.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

CCITT Group 3 팩스 압축을 사용하여 문서를 Tiff 형식의 이미지로 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingCcitt3Compression.tiff");

// 문서를 저장합니다.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          ColorMode = ColorMode.BlackAndWhite,
                          TiffCompression = TiffCompression.Ccitt3
                      });
```

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

* 네임스페이스 [Aspose.Note](../../aspose.note/)
* 집회 [Aspose.Note](../../)


