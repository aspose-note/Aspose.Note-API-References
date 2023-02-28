---
title: SaveOptions.PageIndex
second_title: .NET API 참조용 Aspose.Note
description: SaveOptions 재산. 저장할 첫 번째 페이지의 인덱스를 가져오거나 설정합니다. 기본값은 0. 입니다.
type: docs
weight: 30
url: /ko/net/aspose.note.saving/saveoptions/pageindex/
---
## SaveOptions.PageIndex property

저장할 첫 번째 페이지의 인덱스를 가져오거나 설정합니다. 기본값은 0. 입니다.

```csharp
public int PageIndex { get; set; }
```

### 예

문서를 png 형식으로 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "Aspose.one");

// ImageSaveOptions 객체 초기화 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // 페이지 인덱스 설정
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// 문서를 PNG로 저장합니다.
oneFile.Save(dataDir, opts);
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

문서를 생성하고 지정된 페이지 범위를 html 형식으로 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// OneNote 문서 초기화
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// 문서의 모든 텍스트에 대한 기본 스타일입니다.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// HTML 형식으로 저장
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

서식 있는 서식 있는 텍스트로 문서를 만드는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Document 클래스의 객체 생성
Document doc = new Document();

// 페이지 클래스 객체 초기화
Page page = new Page();

// Title 클래스 객체 초기화
Title title = new Title();

// TextStyle 클래스 개체를 초기화하고 서식 지정 속성을 설정합니다.
ParagraphStyle defaultTextStyle = new ParagraphStyle
                                      {
                                          FontColor = Color.Black,
                                          FontName = "Arial",
                                          FontSize = 10
                                      };

RichText titleText = new RichText() { ParagraphStyle = defaultTextStyle }.Append("Title!");
Outline outline = new Outline()
                      {
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };
OutlineElement outlineElem = new OutlineElement();

TextStyle textStyleForHelloWord = new TextStyle
                                      {
                                          FontColor = Color.Red,
                                          FontName = "Arial",
                                          FontSize = 10,
                                      };

TextStyle textStyleForOneNoteWord = new TextStyle
                                        {
                                            FontColor = Color.Green,
                                            FontName = "Calibri",
                                            FontSize = 10,
                                            IsItalic = true,
                                        };

TextStyle textStyleForTextWord = new TextStyle
                                     {
                                         FontColor = Color.Blue,
                                         FontName = "Arial",
                                         FontSize = 15,
                                         IsBold = true,
                                         IsItalic = true,
                                     };

RichText text = new RichText() { ParagraphStyle = defaultTextStyle }
                    .Append("Hello", textStyleForHelloWord)
                    .Append(" OneNote", textStyleForOneNoteWord)
                    .Append(" text", textStyleForTextWord)
                    .Append("!", TextStyle.Default);

title.TitleText = titleText;

// 페이지 제목 설정
page.Title = title;

// RichText 노드 추가
outlineElem.AppendChildLast(text);

// OutlineElement 노드 추가
outline.AppendChildLast(outlineElem);

// 아웃라인 노드 추가
page.AppendChildLast(outline);

// 페이지 노드 추가
doc.AppendChildLast(page);

// OneNote 문서 저장
dataDir = dataDir + "CreateDocWithFormattedRichText_out.one";
doc.Save(dataDir);
```

### 또한보십시오

* class [SaveOptions](../)
* 네임스페이스 [Aspose.Note.Saving](../../saveoptions/)
* 집회 [Aspose.Note](../../../)


