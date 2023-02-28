---
title: Document.Save
second_title: .NET API 참조용 Aspose.Note
description: Document 방법. OneNote 문서를 파일에 저장합니다.
type: docs
weight: 140
url: /ko/net/aspose.note/document/save/
---
## Save(string) {#save_3}

OneNote 문서를 파일에 저장합니다.

```csharp
public void Save(string fileName)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| fileName | String | 파일의 전체 이름입니다. 지정된 전체 이름을 가진 파일이 이미 존재하는 경우 기존 파일을 덮어씁니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | 문서 구조가 사양을 위반합니다. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | 요청한 저장 형식이 지원되지 않습니다. |

### 예

문서를 저장하는 방법을 보여줍니다.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

### 또한보십시오

* class [Document](../)
* 네임스페이스 [Aspose.Note](../../document/)
* 집회 [Aspose.Note](../../../)

---

## Save(Stream) {#save}

OneNote 문서를 스트림에 저장합니다.

```csharp
public void Save(Stream stream)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| stream | Stream | 문서가 저장될 System.IO.Stream입니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | 문서 구조가 사양을 위반합니다. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | 요청한 저장 형식이 지원되지 않습니다. |

### 또한보십시오

* class [Document](../)
* 네임스페이스 [Aspose.Note](../../document/)
* 집회 [Aspose.Note](../../../)

---

## Save(string, SaveFormat) {#save_4}

OneNote 문서를 지정된 형식의 파일로 저장합니다.

```csharp
public void Save(string fileName, SaveFormat format)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| fileName | String | 파일의 전체 이름입니다. 지정된 전체 이름을 가진 파일이 이미 존재하는 경우 기존 파일을 덮어씁니다. |
| format | SaveFormat | 문서를 저장할 형식입니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | 문서 구조가 사양을 위반합니다. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | 요청한 저장 형식이 지원되지 않습니다. |

### 예

SaveFormat 열거형을 사용하여 문서를 저장하는 방법을 보여줍니다.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
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

### 또한보십시오

* enum [SaveFormat](../../saveformat/)
* class [Document](../)
* 네임스페이스 [Aspose.Note](../../document/)
* 집회 [Aspose.Note](../../../)

---

## Save(Stream, SaveFormat) {#save_1}

OneNote 문서를 지정된 형식의 스트림에 저장합니다.

```csharp
public void Save(Stream stream, SaveFormat format)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| stream | Stream | 문서가 저장될 System.IO.Stream입니다. |
| format | SaveFormat | 문서를 저장할 형식입니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | 문서 구조가 사양을 위반합니다. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | 요청한 저장 형식이 지원되지 않습니다. |

### 예

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

문서를 스트림에 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// 스트림 위치를 다시 0으로 되감아 다음 판독기를 준비합니다.
dstStream.Seek(0, SeekOrigin.Begin);
```

어두운 테마 스타일을 문서에 적용하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Text();

// 문서를 Aspose.Note에 로드합니다.
Document doc = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in doc)
{
    page.BackgroundColor = Color.Black;
}

foreach (var node in doc.GetChildNodes<RichText>())
{
    var c = node.ParagraphStyle.FontColor;
    if (c.IsEmpty || Math.Abs(c.R - Color.Black.R) + Math.Abs(c.G - Color.Black.G) + Math.Abs(c.B - Color.Black.B) <= 30)
    {
        node.ParagraphStyle.FontColor = Color.White;
    }
}

doc.Save(Path.Combine(dataDir, "AsposeDarkTheme.pdf"));
```

### 또한보십시오

* enum [SaveFormat](../../saveformat/)
* class [Document](../)
* 네임스페이스 [Aspose.Note](../../document/)
* 집회 [Aspose.Note](../../../)

---

## Save(string, SaveOptions) {#save_5}

지정된 저장 옵션을 사용하여 OneNote 문서를 파일로 저장합니다.

```csharp
public void Save(string fileName, SaveOptions options)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| fileName | String | 파일의 전체 이름입니다. 지정된 전체 이름을 가진 파일이 이미 존재하는 경우 기존 파일을 덮어씁니다. |
| options | SaveOptions | 문서가 파일에 저장되는 옵션을 지정합니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | 문서 구조가 사양을 위반합니다. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | 요청한 저장 형식이 지원되지 않습니다. |

### 예

OneSaveOptions를 사용하여 문서를 저장하는 방법을 보여줍니다.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
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

Letter 페이지 레이아웃을 사용하여 PDF 형식으로 문서를 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// 문서를 저장합니다.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

높이 제한 없이 A4 페이지 레이아웃으로 PDF 형식으로 문서를 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// 문서를 저장합니다.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
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

PDF 형식으로 문서를 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "Aspose.one");

// PdfSaveOptions 객체 초기화
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // 저장할 첫 번째 페이지의 페이지 인덱스 설정
                              PageIndex = 0,

                              // 페이지 수 설정
                              PageCount = 1,
                          };

// 문서를 PDF로 저장
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

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

* class [SaveOptions](../../../aspose.note.saving/saveoptions/)
* class [Document](../)
* 네임스페이스 [Aspose.Note](../../document/)
* 집회 [Aspose.Note](../../../)

---

## Save(Stream, SaveOptions) {#save_2}

지정된 저장 옵션을 사용하여 OneNote 문서를 스트림에 저장합니다.

```csharp
public void Save(Stream stream, SaveOptions options)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| stream | Stream | 문서가 저장될 System.IO.Stream입니다. |
| options | SaveOptions | 문서가 스트림에 저장되는 옵션을 지정합니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | 문서 구조가 사양을 위반합니다. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | 요청한 저장 형식이 지원되지 않습니다. |

### 예

지정된 기본 글꼴을 사용하여 PDF 형식으로 문서를 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// 문서를 PDF로 저장
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

파일의 기본 글꼴을 사용하여 PDF 형식으로 문서를 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// 문서를 PDF로 저장
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

스트림의 기본 글꼴을 사용하여 PDF 형식으로 문서를 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// 문서를 PDF로 저장
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### 또한보십시오

* class [SaveOptions](../../../aspose.note.saving/saveoptions/)
* class [Document](../)
* 네임스페이스 [Aspose.Note](../../document/)
* 집회 [Aspose.Note](../../../)


