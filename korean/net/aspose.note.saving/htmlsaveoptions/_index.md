---
title: Class HtmlSaveOptions
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.Saving.HtmlSaveOptions 수업. 문서를 HTML 형식으로 저장할 때 추가 옵션을 지정할 수 있습니다.
type: docs
weight: 700
url: /ko/net/aspose.note.saving/htmlsaveoptions/
---
## HtmlSaveOptions class

문서를 HTML 형식으로 저장할 때 추가 옵션을 지정할 수 있습니다.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions/)() | 기본 생성자입니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [CssPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/cssperpagegeneration/) { get; set; } | 각 새 페이지에 대해 별도로 StyleSheet 파일을 생성할지 여부를 가져오거나 설정합니다. |
| [CssSavingCallback](../../aspose.note.saving/htmlsaveoptions/csssavingcallback/) { get; set; } | CSS를 저장할 리소스를 생성하기 위해 호출되는 콜백을 가져오거나 설정합니다. |
| [DocumentPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/documentperpagegeneration/) { get; set; } | 페이지당 문서 생성이 활성화되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [ExportCss](../../aspose.note.saving/htmlsaveoptions/exportcss/) { get; set; } | CSS를 내보내는 방법을 가져오거나 설정합니다. |
| [ExportFonts](../../aspose.note.saving/htmlsaveoptions/exportfonts/) { get; set; } | 글꼴을 내보내는 방법을 가져오거나 설정합니다. |
| [ExportImages](../../aspose.note.saving/htmlsaveoptions/exportimages/) { get; set; } | 이미지를 내보내는 방법을 가져오거나 설정합니다. |
| [FontFaceTypes](../../aspose.note.saving/htmlsaveoptions/fontfacetypes/) { get; set; } | 글꼴 유형을 가져오거나 설정합니다. |
| [FontSavingCallback](../../aspose.note.saving/htmlsaveoptions/fontsavingcallback/) { get; set; } | 글꼴을 저장할 리소스를 생성하기 위해 호출되는 콜백을 가져오거나 설정합니다. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | 를 저장하는 동안 사용할 글꼴 설정을 가져오거나 설정합니다. |
| [ImageSavingCallback](../../aspose.note.saving/htmlsaveoptions/imagesavingcallback/) { get; set; } | 이미지를 저장할 리소스를 생성하기 위해 호출되는 콜백을 가져오거나 설정합니다. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | 저장할 페이지 수를 가져오거나 설정합니다. 기본적으로MaxValue 문서의 모든 페이지가 렌더링됨을 의미합니다. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | 저장할 첫 번째 페이지의 인덱스를 가져오거나 설정합니다. 기본값은 0. 입니다. |
| [PageSavingCallback](../../aspose.note.saving/htmlsaveoptions/pagesavingcallback/) { get; set; } | 페이지를 저장할 리소스를 생성하기 위해 호출되는 콜백을 가져오거나 설정합니다. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | 문서가 저장되는 형식을 가져옵니다. |

### 예

모든 리소스(css/fonts/images)를 별도의 파일에 저장하여 문서를 html 형식으로 저장하는 방법을 보여줍니다.

```csharp
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

var options = new HtmlSaveOptions()
             {
                 ExportCss = ResourceExportType.ExportAsStream,
                 ExportFonts = ResourceExportType.ExportAsStream,
                 ExportImages = ResourceExportType.ExportAsStream,
                 FontFaceTypes = FontFaceType.Ttf
             };
document.Save(dataDir + "document_out.html", options);
```

모든 리소스(css/fonts/images)를 포함하여 html 형식의 스트림에 문서를 저장하는 방법을 보여줍니다.

```csharp
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

var options = new HtmlSaveOptions()
             {
                 ExportCss = ResourceExportType.ExportEmbedded,
                 ExportFonts = ResourceExportType.ExportEmbedded,
                 ExportImages = ResourceExportType.ExportEmbedded,
                 FontFaceTypes = FontFaceType.Ttf
             };

var r = new MemoryStream();
document.Save(r, options);
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

사용자 정의 콜백을 사용하여 모든 리소스(css/fonts/images)를 저장하여 html 형식으로 문서를 저장하는 방법을 보여줍니다.

```csharp
// 아래 코드는 document.html이 포함된 'documentFolder' 폴더, 'style.css' 파일이 포함된 'css' 폴더, 이미지가 포함된 'images' 폴더, 글꼴이 포함된 'fonts' 폴더를 생성합니다.
// 'style.css' 파일은 끝에 다음 문자열을 포함합니다. "/* 이 줄은 사용자가 수동으로 스트림에 추가합니다 */"
var savingCallbacks = new UserSavingCallbacks()
                          {
                              RootFolder = "documentFolder",
                              CssFolder = "css",
                              KeepCssStreamOpened = true,
                              ImagesFolder = "images",
                              FontsFolder = "fonts"
                          };
var options = new HtmlSaveOptions
              {
                  FontFaceTypes = FontFaceType.Ttf,
                  CssSavingCallback = savingCallbacks,
                  FontSavingCallback = savingCallbacks,
                  ImageSavingCallback = savingCallbacks
              };

if (!Directory.Exists(savingCallbacks.RootFolder))
{
    Directory.CreateDirectory(savingCallbacks.RootFolder);
}

string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

using (var stream = File.Create(Path.Combine(savingCallbacks.RootFolder, "document.html")))
{
    document.Save(stream, options);
}

using (var writer = new StreamWriter(savingCallbacks.CssStream))
{
    writer.WriteLine();
    writer.WriteLine("/* This line is appended to stream manually by user */");
}
```

### 또한보십시오

* class [SaveOptions](../saveoptions/)
* 네임스페이스 [Aspose.Note.Saving](../../aspose.note.saving/)
* 집회 [Aspose.Note](../../)


