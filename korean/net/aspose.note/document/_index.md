---
title: Class Document
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.Document 수업. Aspose.Note 문서를 나타냅니다.
type: docs
weight: 60
url: /ko/net/aspose.note/document/
---
## Document class

Aspose.Note 문서를 나타냅니다.

```csharp
public class Document : CompositeNode<Page>, INotebookChildNode
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [Document](document/#constructor)() | 의 새 인스턴스를 초기화합니다.`Document` class. 빈 OneNote 문서를 만듭니다. |
| [Document](document/#constructor_1)(Stream) | 의 새 인스턴스를 초기화합니다.`Document` class. 스트림에서 기존 OneNote 문서를 엽니다. |
| [Document](document/#constructor_3)(string) | 의 새 인스턴스를 초기화합니다.`Document` class. 파일에서 기존 OneNote 문서를 엽니다. |
| [Document](document/#constructor_2)(Stream, LoadOptions) | 의 새 인스턴스를 초기화합니다.`Document` class. 스트림에서 기존 OneNote 문서를 엽니다. 암호화 암호와 같은 추가 옵션을 지정할 수 있습니다. |
| [Document](document/#constructor_4)(string, LoadOptions) | 의 새 인스턴스를 초기화합니다.`Document`class. 파일에서 기존 OneNote 문서를 엽니다. 암호화 암호와 같은 추가 옵션을 지정할 수 있습니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [AutomaticLayoutChangesDetectionEnabled](../../aspose.note/document/automaticlayoutchangesdetectionenabled/) { get; set; } | Aspose.Note가 레이아웃 변경을 자동으로 감지하는지 여부를 나타내는 값을 가져오거나 설정합니다. 기본값은`진실` . |
| [Color](../../aspose.note/document/color/) { get; set; } | 색상을 가져오거나 설정합니다. |
| [CreationTime](../../aspose.note/document/creationtime/) { get; set; } | 생성 시간을 가져오거나 설정합니다. |
| [DisplayName](../../aspose.note/document/displayname/) { get; set; } | 표시 이름을 가져오거나 설정합니다. |
| [Document](../../aspose.note/node/document/) { get; } | 노드의 문서를 가져옵니다. |
| [FileFormat](../../aspose.note/document/fileformat/) { get; } | 파일 형식 가져오기(OneNote 2010, OneNote Online). |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [Guid](../../aspose.note/document/guid/) { get; } | 개체의 전역 고유 ID를 가져옵니다. |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | 동일한 노드 트리 수준에서 다음 노드를 가져옵니다. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | 노드 유형을 가져옵니다. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | 상위 노드를 가져옵니다. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | 동일한 노드 트리 수준에서 이전 노드를 가져옵니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| override [Accept](../../aspose.note/document/accept/)(DocumentVisitor) | 노드의 방문자를 수락합니다. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| [DetectLayoutChanges](../../aspose.note/document/detectlayoutchanges/)() | 이전 이후 문서 레이아웃에 대한 모든 변경 사항을 감지합니다.[`DetectLayoutChanges`](./detectlayoutchanges/) call. 만일의 경우[`AutomaticLayoutChangesDetectionEnabled`](./automaticlayoutchangesdetectionenabled/) true로 설정하면 문서 내보내기 시작 시 자동으로 사용됩니다. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| [GetPageHistory](../../aspose.note/document/getpagehistory/)(Page) | 가져오기[`PageHistory`](../pagehistory/) 문서에 표시된 각 페이지에 대한 전체 기록을 포함합니다(가장 빠른 인덱스 0). 현재 페이지 개정판은 다음과 같이 액세스할 수 있습니다.[`Current`](../pagehistory/current/) 기록 버전 컬렉션과 별도로 포함됩니다. |
| [Import](../../aspose.note/document/import/#import)(Stream, PdfImportOptions, MergeOptions) | 제공된 PDF 문서에서 페이지 세트를 가져옵니다. |
| [Import](../../aspose.note/document/import/#import_1)(string, PdfImportOptions, MergeOptions) | 제공된 PDF 문서에서 페이지 세트를 가져옵니다. |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;Page&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params Page[]) |  |
| [Merge](../../aspose.note/document/merge/)(IEnumerable&lt;Page&gt;, MergeOptions) | 페이지 집합을 문서에 병합합니다. |
| [Print](../../aspose.note/document/print/#print)() | 기본 프린터를 사용하여 문서를 인쇄합니다. |
| [Print](../../aspose.note/document/print/#print_1)(PrintOptions) | 기본 프린터를 사용하여 문서를 인쇄합니다. |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |
| [Save](../../aspose.note/document/save/#save)(Stream) | OneNote 문서를 스트림에 저장합니다. |
| [Save](../../aspose.note/document/save/#save_3)(string) | OneNote 문서를 파일에 저장합니다. |
| [Save](../../aspose.note/document/save/#save_1)(Stream, SaveFormat) | OneNote 문서를 지정된 형식의 스트림에 저장합니다. |
| [Save](../../aspose.note/document/save/#save_2)(Stream, SaveOptions) | 지정된 저장 옵션을 사용하여 OneNote 문서를 스트림에 저장합니다. |
| [Save](../../aspose.note/document/save/#save_4)(string, SaveFormat) | OneNote 문서를 지정된 형식의 파일로 저장합니다. |
| [Save](../../aspose.note/document/save/#save_5)(string, SaveOptions) | 지정된 저장 옵션을 사용하여 OneNote 문서를 파일로 저장합니다. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted)(Stream, out Document) | 스트림의 문서가 암호화되었는지 확인합니다. 확인하려면 이 문서를 완전히 로드해야 합니다. 따라서 이 방법은 성능 저하로 이어질 수 있습니다. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_3)(string, out Document) | 파일의 문서가 암호화되었는지 확인합니다. 확인하려면 이 문서를 완전히 로드해야 합니다. 따라서 이 방법은 성능 저하로 이어질 수 있습니다. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_1)(Stream, LoadOptions, out Document) | 스트림의 문서가 암호화되었는지 확인합니다. 확인하려면 이 문서를 완전히 로드해야 합니다. 따라서 이 방법은 성능 저하로 이어질 수 있습니다. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_2)(Stream, string, out Document) | 스트림의 문서가 암호화되었는지 확인합니다. 확인하려면 이 문서를 완전히 로드해야 합니다. 따라서 이 방법은 성능 저하로 이어질 수 있습니다. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_4)(string, LoadOptions, out Document) | 파일의 문서가 암호화되었는지 확인합니다. 확인하려면 이 문서를 완전히 로드해야 합니다. 따라서 이 방법은 성능 저하로 이어질 수 있습니다. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_5)(string, string, out Document) | 파일의 문서가 암호화되었는지 확인합니다. 확인하려면 이 문서를 완전히 로드해야 합니다. 따라서 이 방법은 성능 저하로 이어질 수 있습니다. |

### 예

기본 옵션이 있는 표준 Windows 대화 상자를 사용하여 문서를 프린터로 보내는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
```

문서를 저장하는 방법을 보여줍니다.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

문서를 암호화하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

암호화로 문서를 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

SaveFormat 열거형을 사용하여 문서를 저장하는 방법을 보여줍니다.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

OneSaveOptions를 사용하여 문서를 저장하는 방법을 보여줍니다.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

문서의 페이지 수를 가져오는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Pages();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "Aspose.one");

// 페이지 수 얻기
int count = oneFile.Count();

// 출력 화면에 카운트 출력
Console.WriteLine(count);
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

문서의 파일 형식을 가져오는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");
switch (document.FileFormat)
{
    case FileFormat.OneNote2010:
        // OneNote 2010 처리
        break;
    case FileFormat.OneNoteOnline:
        // OneNote 온라인 처리
        break;
}
```

이미지에 하이퍼링크를 바인딩하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://image.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
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

문서가 암호로 보호되어 있는지 확인하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

노트북에 새 섹션을 추가하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote 전자 필기장 로드
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// 새 자식을 노트북에 추가
notebook.AppendChild(new Document(dataDir + "Neuer Abschnitt 1.one"));

dataDir = dataDir + "AddChildNode_out.onetoc2";

// 노트북 저장
notebook.Save(dataDir);
```

OneNote 2007 형식이 지원되지 않아 문서 로드가 실패했는지 확인하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "OneNote2007.one");

try
{
    new Document(fileName);
}
catch (UnsupportedFileFormatException e)
{
    if (e.FileFormat == FileFormat.OneNote2007)
    {
        Console.WriteLine("It looks like the provided file is in OneNote 2007 format that is not supported.");
    }
    else
        throw;
}
```

페이지의 이전 버전을 복원하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote 문서를 로드하고 첫 번째 자식 가져오기           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;           
Page previousPageVersion = document.GetPageHistory(page).Last();

document.RemoveChild(page);
document.AppendChildLast(previousPageVersion);

document.Save(dataDir + "RollBackRevisions_out.one");
```

페이지를 복제하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote 문서 로드
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// 기록 없이 새 문서로 복제
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// 기록이 있는 새 문서로 복제
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

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

이미지에 대한 텍스트 설명을 설정하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Images();

var document = new Document();
var page = new Page(document);
var image = new Image(document, dataDir + "image.jpg")
            {
                AlternativeTextTitle = "This is an image's title!",
                AlternativeTextDescription = "And this is an image's description!"
            };
page.AppendChildLast(image);
document.AppendChildLast(page);

dataDir = dataDir + "ImageAlternativeText_out.one";
document.Save(dataDir);
```

페이지에 대한 메타 정보를 얻는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Pages();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "Aspose.one");

foreach (Page page in oneFile)
{
    Console.WriteLine("LastModifiedTime: {0}", page.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", page.CreationTime);
    Console.WriteLine("Title: {0}", page.Title);
    Console.WriteLine("Level: {0}", page.Level);
    Console.WriteLine("Author: {0}", page.Author);
    Console.WriteLine();
}
```

긴 OneNote 페이지가 pdf 형식으로 저장되면 여러 페이지로 분할됩니다. 이 샘플은 페이지 나누기에 있는 개체의 분할 논리를 구성하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// 또는
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

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

페이지 기록을 편집하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote 문서를 로드하고 첫 번째 자식 가져오기           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.RemoveRange(0, 1);

pageHistory[0] = new Page(document);
if (pageHistory.Count > 1)
{
    pageHistory[1].Title.TitleText.Text = "New Title";

    pageHistory.Add(new Page(document));

    pageHistory.Insert(1, new Page(document));

    document.Save(dataDir + "ModifyPageHistory_out.one");
}
```

문서가 특정 암호로 암호로 보호되어 있는지 확인하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
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

노트북의 콘텐츠를 전달하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = "Open Notebook.onetoc2";
try
{
    var notebook = new Notebook(dataDir + fileName);
    foreach (var notebookChildNode in notebook)
    {
        Console.WriteLine(notebookChildNode.DisplayName);
        if (notebookChildNode is Document)
        {
            // 하위 문서로 작업 수행
        }
        else if (notebookChildNode is Notebook)
        {
            // 자식 노트북으로 작업 수행
        }
    }
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
```

문서에서 이미지를 가져오는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Images();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "Aspose.one");

// 모든 이미지 노드 가져오기
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // 이미지 바이트를 파일에 저장
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
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

지정된 옵션과 함께 표준 Windows 대화 상자를 사용하여 문서를 프린터로 보내는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

var printerSettings = new PrinterSettings() { FromPage = 0, ToPage = 10 };
printerSettings.DefaultPageSettings.Landscape = true;
printerSettings.DefaultPageSettings.Margins = new System.Drawing.Printing.Margins(50, 50, 150, 50);

document.Print(new PrintOptions()
               {
                   PrinterSettings = printerSettings,
                   Resolution = 1200,
                   PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(),
                   DocumentName = "Test.one"
               });
```

첨부 파일의 내용을 가져오는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Attachments();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "Sample1.one");

// 첨부 파일 노드 목록 가져오기
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// 모든 노드를 반복합니다.
foreach (AttachedFile file in nodes)
{
    // 첨부 파일을 스트림 객체에 로드
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // 로컬 파일 생성
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // 파일 스트림 복사
            CopyStream(outputStream, fileStream);
        }
    }
}
```

이미지의 메타 정보를 가져오는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Images();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "Aspose.one");

// 모든 이미지 노드 가져오기
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

페이지 기록을 가져오는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote 문서 로드
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// 첫 페이지 가져오기
Page firstPage = document.FirstChild;
foreach (Page pageRevision in document.GetPageHistory(firstPage))
{
    /*Use pageRevision like a regular page.*/
    Console.WriteLine("LastModifiedTime: {0}", pageRevision.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", pageRevision.CreationTime);
    Console.WriteLine("Title: {0}", pageRevision.Title);
    Console.WriteLine("Level: {0}", pageRevision.Level);
    Console.WriteLine("Author: {0}", pageRevision.Author);
    Console.WriteLine();
}
```

파일 경로를 사용하여 문서에 파일을 추가하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Attachments();

// Document 클래스의 객체 생성
Document doc = new Document();

// 페이지 클래스 객체 초기화
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 아웃라인 클래스 객체 초기화
Outline outline = new Outline(doc);

// OutlineElement 클래스 객체 초기화
OutlineElement outlineElem = new OutlineElement(doc);

// AttachedFile 클래스 객체 초기화
AttachedFile attachedFile = new AttachedFile(doc,  dataDir + "attachment.txt");

// 첨부파일 추가
outlineElem.AppendChildLast(attachedFile);

// 아웃라인 요소 노드 추가
outline.AppendChildLast(outlineElem);

// 아웃라인 노드 추가
page.AppendChildLast(outline);

// 페이지 노드 추가
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileByPath_out.one";
doc.Save(dataDir);
```

문서를 만들고 기본 옵션을 사용하여 html 형식으로 저장하는 방법을 보여줍니다.

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
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

페이지가 충돌 페이지인지(예: OneNote에서 자동으로 병합할 수 없는 변경 사항이 있음) 확인하는 방법을 보여줍니다.

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote 문서 로드
Document doc = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

var history = doc.GetPageHistory(doc.FirstChild);
for (int i = 0; i < history.Count; i++)
{
    var historyPage = history[i];
    Console.Write("    {0}. Author: {1}, {2:dd.MM.yyyy hh.mm.ss}",
                    i,
                    historyPage.PageContentRevisionSummary.AuthorMostRecent,
                    historyPage.PageContentRevisionSummary.LastModifiedTime);
    Console.WriteLine(historyPage.IsConflictPage ? ", IsConflict: true" : string.Empty);

    // 기본적으로 충돌 페이지는 저장할 때 건너뜁니다.
    // 비충돌로 표시하면 평소와 같이 히스토리에 저장됩니다.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

사용자 정의 속성을 사용하여 파일의 이미지를 문서에 추가하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Images();

// 스트림에서 문서를 로드합니다.
Document doc = new Document(dataDir + "Aspose.one");

// 문서의 첫 번째 페이지를 가져옵니다.
Aspose.Note.Page page = doc.FirstChild;

// 파일에서 이미지를 로드합니다.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // 필요에 따라 이미지 크기를 변경합니다(선택 사항).
                              Width = 100,
                              Height = 100,

                              // 페이지에서 이미지의 위치를 설정합니다(선택 사항).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // 이미지 정렬 설정
                              Alignment = HorizontalAlignment.Right
                          };

// 페이지에 이미지를 추가합니다.
page.AppendChildLast(image);
```

스트림에서 문서로 파일을 추가하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Attachments();

// Document 클래스의 객체 생성
Document doc = new Document();

// 페이지 클래스 객체 초기화
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 아웃라인 클래스 객체 초기화
Outline outline = new Outline(doc);

// OutlineElement 클래스 객체 초기화
OutlineElement outlineElem = new OutlineElement(doc);

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // AttachedFile 클래스 개체를 초기화하고 해당 아이콘 경로도 전달합니다.
    AttachedFile attachedFile = new AttachedFile(doc, dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // 첨부파일 추가
    outlineElem.AppendChildLast(attachedFile);
}

// 아웃라인 요소 노드 추가
outline.AppendChildLast(outlineElem);

// 아웃라인 노드 추가
page.AppendChildLast(outline);

// 페이지 노드 추가
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileAndSetIcon_out.one";
doc.Save(dataDir);
```

긴 OneNote 페이지가 pdf 형식으로 저장되면 여러 페이지로 분할됩니다. 이 예는 페이지 나누기에 있는 개체의 분할 논리를 구성하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// 또는
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// 또는
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// 또는
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// 또는
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
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

제목 페이지가 있는 문서를 만드는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Document 클래스의 객체 생성
Document doc = new Aspose.Note.Document();

// 페이지 클래스 객체 초기화
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 문서의 모든 텍스트에 대한 기본 스타일입니다.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 페이지 제목 속성 설정
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// 문서에 페이지 노드 추가
doc.AppendChildLast(page);

// OneNote 문서 저장
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

스트림에서 문서로 이미지를 추가하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Images();

// Document 클래스의 객체 생성
Document doc = new Document();

// 페이지 클래스 객체 초기화
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // 이미지 이름, 확장자 및 스트림을 사용하여 두 번째 이미지를 로드합니다.
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // 이미지 정렬 설정
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// OneNote 문서 저장
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

파일에서 문서로 이미지를 추가하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Images();

// Document 클래스의 객체 생성
Document doc = new Document();

// 페이지 클래스 객체 초기화
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline 클래스 객체 초기화 및 오프셋 속성 설정
Outline outline = new Outline(doc);

// OutlineElement 클래스 객체 초기화
OutlineElement outlineElem = new OutlineElement(doc);

// 파일 경로로 이미지를 로드합니다.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // 이미지 정렬 설정
                              Alignment = HorizontalAlignment.Right
                          };

// 이미지 추가
outlineElem.AppendChildLast(image);

// 아웃라인 요소 추가
outline.AppendChildLast(outlineElem);

// 아웃라인 노드 추가
page.AppendChildLast(outline);

// 페이지 노드 추가
doc.AppendChildLast(page);

// OneNote 문서 저장
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

텍스트가 포함된 문서를 만드는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Document 클래스의 객체 생성
Document doc = new Document();

// 페이지 클래스 객체 초기화
Page page = new Page(doc);

// 아웃라인 클래스 객체 초기화
Outline outline = new Outline(doc);

// OutlineElement 클래스 객체 초기화
OutlineElement outlineElem = new OutlineElement(doc);

// TextStyle 클래스 개체를 초기화하고 서식 지정 속성을 설정합니다.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// RichText 클래스 객체 초기화 및 텍스트 스타일 적용
RichText text = new RichText(doc) { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// RichText 노드 추가
outlineElem.AppendChildLast(text);

// OutlineElement 노드 추가
outline.AppendChildLast(outlineElem);

// 아웃라인 노드 추가
page.AppendChildLast(outline);

// 페이지 노드 추가
doc.AppendChildLast(page);

// OneNote 문서 저장
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
doc.Save(dataDir);
```

다양한 형식으로 문서를 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 새 문서 초기화
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// 새 페이지 초기화
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 문서의 모든 텍스트에 대한 기본 스타일입니다.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// 페이지 노드 추가
doc.AppendChildLast(page);

// OneNote 문서를 다른 형식으로 저장하고, 텍스트 글꼴 크기를 설정하고, 레이아웃 변경을 수동으로 감지합니다.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
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

하이퍼링크를 텍스트에 바인딩하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Tasks();

// Document 클래스의 객체 생성
Document doc = new Document();

RichText titleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append("Title!");

Outline outline = new Outline()
                      {
                          MaxWidth = 200,
                          MaxHeight = 200,
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };

TextStyle textStyleRed = new TextStyle
                             {
                                 FontColor = Color.Red,
                                 FontName = "Arial",
                                 FontSize = 10,
                             };

TextStyle textStyleHyperlink = new TextStyle
                                   {
                                       IsHyperlink = true,
                                       HyperlinkAddress = "www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// 아웃라인 요소 추가
outline.AppendChildLast(outlineElem);

// Title 클래스 객체 초기화
Title title = new Title() { TitleText = titleText };

// 페이지 클래스 객체 초기화
Page page = new Note.Page() { Title = title };

// 아웃라인 노드 추가
page.AppendChildLast(outline);

// 페이지 노드 추가
doc.AppendChildLast(page);

// OneNote 문서 저장
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

방문자를 사용하여 문서의 콘텐츠에 액세스하는 방법을 보여줍니다.

```csharp
public static void Run()
{
    // 문서 디렉토리의 경로.
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // 변환하려는 문서를 엽니다.
    Document doc = new Document(dataDir + "Aspose.one");

    // DocumentVisitor 클래스에서 상속되는 객체를 생성합니다.
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // 이것은 잘 알려진 방문자 패턴입니다. 방문자를 받아들이도록 모델을 가져오십시오.
    // 모델은 해당 메소드를 호출하여 자체적으로 반복합니다.
    // 방문자 개체에 대해(이를 방문이라고 함).
    //
    // 객체 모델의 모든 노드에는 Accept 메서드가 있으므로 방문하는
    // 전체 문서뿐만 아니라 문서의 모든 노드에 대해 실행할 수 있습니다.
    doc.Accept(myConverter);

    // 방문이 완료되면 작업 결과를 검색할 수 있습니다.
    // 이 예에서는 방문자에 누적되었습니다.
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// 일반 텍스트 형식으로 문서를 저장하는 간단한 구현입니다. 방문자로 구현됩니다.
/// </summary>
public class MyOneNoteToTxtWriter : DocumentVisitor
{
    public MyOneNoteToTxtWriter()
    {
        nodecount = 0;
        mIsSkipText = false;
        mBuilder = new StringBuilder();
    }

    /// <summary>
    /// 방문자가 축적한 문서의 일반 텍스트를 가져옵니다.
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// 현재 출력에 텍스트를 추가합니다. 활성화/비활성화 출력 플래그를 존중합니다.
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// RichText 노드가 문서에서 발견될 때 호출됩니다.
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// Document 노드가 문서에서 발견될 때 호출됩니다.
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// 문서에서 페이지 노드를 만나면 호출됩니다.
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// 페이지 노드의 처리가 완료되면 호출됩니다.
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// 문서에서 Title 노드를 만나면 호출됩니다.
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// 문서에서 이미지 노드를 만났을 때 호출됩니다.
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// 문서에서 OutlineGroup 노드를 만나면 호출됩니다.
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// 문서에서 아웃라인 노드를 만나면 호출됩니다.
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// 문서에서 OutlineElement 노드를 만나면 호출됩니다.
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// 방문자의 총 노드 수를 가져옵니다.
    /// </summary>
    public Int32 NodeCount
    {
        get { return this.nodecount; }
    }

    private readonly StringBuilder mBuilder;
    private bool mIsSkipText;
    private Int32 nodecount;
}
```

### 또한보십시오

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* class [Page](../page/)
* interface [INotebookChildNode](../inotebookchildnode/)
* 네임스페이스 [Aspose.Note](../../aspose.note/)
* 집회 [Aspose.Note](../../)


