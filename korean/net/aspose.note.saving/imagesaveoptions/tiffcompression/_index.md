---
title: ImageSaveOptions.TiffCompression
second_title: .NET API 참조용 Aspose.Note
description: ImageSaveOptions 재산. 생성된 이미지를 TIFF 형식으로 저장할 때 사용할 압축 유형을 가져오거나 설정합니다.
type: docs
weight: 60
url: /ko/net/aspose.note.saving/imagesaveoptions/tiffcompression/
---
## ImageSaveOptions.TiffCompression property

생성된 이미지를 TIFF 형식으로 저장할 때 사용할 압축 유형을 가져오거나 설정합니다.

```csharp
public TiffCompression TiffCompression { get; set; }
```

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

* enum [TiffCompression](../../tiffcompression/)
* class [ImageSaveOptions](../)
* 네임스페이스 [Aspose.Note.Saving](../../imagesaveoptions/)
* 집회 [Aspose.Note](../../../)


