---
title: PdfSaveOptions.JpegQuality
second_title: .NET API 참조용 Aspose.Note
description: PdfSaveOptions 재산. PDF 문서 내 JPEG 이미지의 품질을 결정하는 값을 가져오거나 설정합니다. 값은 0에서 100까지 다양할 수 있습니다. 여기서 0은 품질이 가장 낮지만 최대 압축률을 의미하고 100은 최상의 품질이지만 최소 압축률을 의미합니다.
type: docs
weight: 30
url: /ko/net/aspose.note.saving/pdfsaveoptions/jpegquality/
---
## PdfSaveOptions.JpegQuality property

PDF 문서 내 JPEG 이미지의 품질을 결정하는 값을 가져오거나 설정합니다. 값은 0에서 100까지 다양할 수 있습니다. 여기서 0은 품질이 가장 낮지만 최대 압축률을 의미하고 100은 최상의 품질이지만 최소 압축률을 의미합니다.

```csharp
public int JpegQuality { get; set; }
```

### 비고

기본값은 90입니다.

### 예

특정 설정을 사용하여 문서를 PDF 형식으로 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document doc = new Document(dataDir + "Aspose.one");

// PdfSaveOptions 객체 초기화
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Jpeg 압축 사용
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // JPEG 압축 품질
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

### 또한보십시오

* class [PdfSaveOptions](../)
* 네임스페이스 [Aspose.Note.Saving](../../pdfsaveoptions/)
* 집회 [Aspose.Note](../../../)


