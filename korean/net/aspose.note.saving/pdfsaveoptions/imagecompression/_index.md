---
title: PdfSaveOptions.ImageCompression
second_title: .NET API 참조용 Aspose.Note
description: PdfSaveOptions 재산. PDF 파일의 이미지에 적용되는 압축 유형을 가져오거나 설정합니다.
type: docs
weight: 20
url: /ko/net/aspose.note.saving/pdfsaveoptions/imagecompression/
---
## PdfSaveOptions.ImageCompression property

PDF 파일의 이미지에 적용되는 압축 유형을 가져오거나 설정합니다.

```csharp
public PdfImageCompression ImageCompression { get; set; }
```

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

* enum [PdfImageCompression](../../../aspose.note.saving.pdf/pdfimagecompression/)
* class [PdfSaveOptions](../)
* 네임스페이스 [Aspose.Note.Saving](../../pdfsaveoptions/)
* 집회 [Aspose.Note](../../../)


