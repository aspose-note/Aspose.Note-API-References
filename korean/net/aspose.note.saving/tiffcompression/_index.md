---
title: Enum TiffCompression
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.Saving.TiffCompression 열거형. 문서를 TIFF 형식으로 저장할 때 사용할 압축 유형을 지정합니다.
type: docs
weight: 880
url: /ko/net/aspose.note.saving/tiffcompression/
---
## TiffCompression enumeration

문서를 TIFF 형식으로 저장할 때 사용할 압축 유형을 지정합니다.

```csharp
public enum TiffCompression
```

### 가치

| 이름 | 값 | 설명 |
| --- | --- | --- |
| None | `1` | 압축을 지정하지 않습니다. |
| Rle | `2` | RLE 압축을 지정합니다. |
| Ccitt3 | `3` | CCITT 그룹 3 팩스 인코딩을 지정합니다. |
| Ccitt4 | `4` | CCITT 그룹 4 팩스 인코딩을 지정합니다. |
| Lzw | `5` | LZW 압축을 지정합니다. |
| PackBits | `32773` | Macintosh RLE 압축을 지정합니다. |
| Jpeg | `7` | JPEG DCT 압축 압축을 지정합니다. |

### 예

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

### 또한보십시오

* 네임스페이스 [Aspose.Note.Saving](../../aspose.note.saving/)
* 집회 [Aspose.Note](../../)


