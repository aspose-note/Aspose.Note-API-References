---
title: ImageSaveOptions.Quality
second_title: .NET API 참조용 Aspose.Note
description: ImageSaveOptions 재산. 저장된 이미지의 품질을 결정하는 값을 가져오거나 설정합니다. 이 값은 코덱에 System.Drawing.Imaging.Encoder.Quality 매개변수로 전달됩니다.
type: docs
weight: 40
url: /ko/net/aspose.note.saving/imagesaveoptions/quality/
---
## ImageSaveOptions.Quality property

저장된 이미지의 품질을 결정하는 값을 가져오거나 설정합니다. 이 값은 코덱에 System.Drawing.Imaging.Encoder.Quality 매개변수로 전달됩니다.

```csharp
public int Quality { get; set; }
```

### 비고

품질 범주에 대한 유용한 값의 범위는 0에서 100까지입니다. 지정된 숫자가 낮을수록 압축률이 높아져 이미지 품질이 낮아집니다. 0은 가장 낮은 품질의 이미지를 제공하고 100은 가장 높은 이미지를 제공합니다. . 기본값은 90입니다.

### 예

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

### 또한보십시오

* class [ImageSaveOptions](../)
* 네임스페이스 [Aspose.Note.Saving](../../imagesaveoptions/)
* 집회 [Aspose.Note](../../../)


