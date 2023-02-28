---
title: Class RichText
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.RichText 수업. 리치 텍스트를 나타냅니다.
type: docs
weight: 530
url: /ko/net/aspose.note/richtext/
---
## RichText class

리치 텍스트를 나타냅니다.

```csharp
public sealed class RichText : Node, IEnumerable<char>, IOutlineElementChildNode, ITaggable
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [RichText](richtext/#constructor)() | 의 새 인스턴스를 초기화합니다.`RichText` 클래스. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Alignment](../../aspose.note/richtext/alignment/) { get; set; } | 정렬을 가져오거나 설정합니다. |
| [Document](../../aspose.note/node/document/) { get; } | 노드의 문서를 가져옵니다. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | 이 노드가 복합인지 여부를 나타내는 값을 가져옵니다. true인 경우 노드에 하위 노드가 있을 수 있습니다. |
| [LastModifiedTime](../../aspose.note/richtext/lastmodifiedtime/) { get; set; } | 마지막 수정 시간을 가져오거나 설정합니다. |
| [Length](../../aspose.note/richtext/length/) { get; } | 텍스트의 길이를 가져옵니다. |
| [LineSpacing](../../aspose.note/richtext/linespacing/) { get; set; } | 줄 간격을 가져오거나 설정합니다. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | 동일한 노드 트리 수준에서 다음 노드를 가져옵니다. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | 노드 유형을 가져옵니다. |
| [ParagraphStyle](../../aspose.note/richtext/paragraphstyle/) { get; set; } | 단락 스타일을 가져오거나 설정합니다. 이 설정은 일치하는 TextStyle 객체가 없는 경우에 사용됩니다.Styles 컬렉션 또는 이 개체가 필요한 설정을 지정하지 않습니다. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | 상위 노드를 가져옵니다. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | 동일한 노드 트리 수준에서 이전 노드를 가져옵니다. |
| [SpaceAfter](../../aspose.note/richtext/spaceafter/) { get; set; } | 이후의 최소 공간을 가져오거나 설정합니다. |
| [SpaceBefore](../../aspose.note/richtext/spacebefore/) { get; set; } | 이전의 최소 공간을 가져오거나 설정합니다. |
| [Tags](../../aspose.note/richtext/tags/) { get; } | 단락의 모든 태그 목록을 가져옵니다. |
| [Text](../../aspose.note/richtext/text/) { get; set; } | 텍스트를 가져오거나 설정합니다. 문자열은 값 10(줄 바꿈)의 문자를 포함하면 안 됩니다. |
| [TextRuns](../../aspose.note/richtext/textruns/) { get; } | 텍스트 실행 모음을 가져옵니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| override [Accept](../../aspose.note/richtext/accept/)(DocumentVisitor) | 노드의 방문자를 수락합니다. |
| [Append](../../aspose.note/richtext/append/#append)(string) | 마지막 텍스트 범위에 문자열을 추가합니다. |
| [Append](../../aspose.note/richtext/append/#append_1)(string, TextStyle) | 끝에 문자열을 추가합니다. |
| [AppendFront](../../aspose.note/richtext/appendfront/#appendfront)(string) | 첫 번째 텍스트 범위 앞에 문자열을 추가합니다. |
| [AppendFront](../../aspose.note/richtext/appendfront/#appendfront_1)(string, TextStyle) | 앞에 문자열을 추가합니다. |
| [Clear](../../aspose.note/richtext/clear/)() | 이 인스턴스의 내용을 지웁니다. |
| [GetEnumerator](../../aspose.note/richtext/getenumerator/)() | 이 RichText 개체의 문자를 반복하는 열거자를 반환합니다. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof)(char) | 이 문자열에서 지정된 유니코드 문자가 처음 나타나는 인덱스(0부터 시작)를 반환합니다. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_3)(string) | 이 인스턴스에서 지정된 문자열이 처음 나타나는 인덱스(0부터 시작)를 반환합니다. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_1)(char, int) | 이 문자열에서 지정된 유니코드 문자가 처음 나타나는 인덱스(0부터 시작)를 반환합니다. 지정된 문자 위치에서 검색을 시작합니다. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_4)(string, int) | 이 인스턴스에서 지정된 문자열이 처음 나타나는 인덱스(0부터 시작)를 반환합니다. 지정된 문자 위치에서 검색을 시작합니다. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_8)(string, StringComparison) | 현재 인스턴스에서 지정된 문자열이 처음 나타나는 인덱스(0부터 시작)를 반환합니다. 매개변수는 지정된 문자열에 사용할 검색 유형을 지정합니다. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_2)(char, int, int) | 이 인스턴스에서 지정된 문자가 처음 나타나는 인덱스(0부터 시작)를 반환합니다. 검색은 지정된 문자 위치에서 시작하여 지정된 수의 문자 위치를 검사합니다. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_5)(string, int, int) | 이 인스턴스에서 지정된 문자열이 처음 나타나는 인덱스(0부터 시작)를 반환합니다. 검색은 지정된 문자 위치에서 시작하여 지정된 수의 문자 위치를 검사합니다. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_7)(string, int, StringComparison) | 현재 인스턴스에서 지정된 문자열이 처음 나타나는 인덱스(0부터 시작)를 반환합니다. 매개변수는 현재 문자열에서 검색 시작 위치와 지정된 문자열에 사용할 검색 유형을 지정합니다. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_6)(string, int, int, StringComparison) | 현재 인스턴스에서 지정된 문자열이 처음 나타나는 인덱스(0부터 시작)를 반환합니다. |
| [Insert](../../aspose.note/richtext/insert/#insert)(int, string) | 이 인스턴스의 지정된 인덱스 위치에 지정된 문자열을 삽입합니다. |
| [Insert](../../aspose.note/richtext/insert/#insert_1)(int, string, TextStyle) | 이 인스턴스의 지정된 인덱스 위치에 지정된 스타일로 지정된 문자열을 삽입합니다. |
| [Remove](../../aspose.note/richtext/remove/#remove)(int) | 지정된 위치에서 시작하여 마지막 위치까지 계속되는 현재 인스턴스의 모든 문자를 제거합니다. |
| [Remove](../../aspose.note/richtext/remove/#remove_1)(int, int) | 지정된 위치에서 시작하여 현재 인스턴스에서 지정된 수의 문자를 제거합니다. |
| [Replace](../../aspose.note/richtext/replace/#replace)(char, char) | 이 인스턴스에서 지정된 유니코드 문자의 모든 항목을 지정된 다른 유니코드 문자로 바꿉니다. |
| [Replace](../../aspose.note/richtext/replace/#replace_1)(string, string) | 현재 인스턴스에서 지정된 문자열의 모든 발생을 다른 지정된 문자열로 바꿉니다. |
| [Replace](../../aspose.note/richtext/replace/#replace_2)(string, string, TextStyle) | 현재 인스턴스에서 지정된 문자열의 모든 항목을 지정된 스타일의 다른 지정된 문자열로 바꿉니다. |
| [Trim](../../aspose.note/richtext/trim/#trim)() | 선행 및 후행 공백 문자를 모두 제거합니다. |
| [Trim](../../aspose.note/richtext/trim/#trim_1)(char) | 문자의 모든 선행 및 후행 인스턴스를 제거합니다. |
| [Trim](../../aspose.note/richtext/trim/#trim_2)(params char[]) | 배열에 지정된 문자 집합의 모든 선행 및 후행 항목을 제거합니다. |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend)() | 후행 공백 문자를 모두 제거합니다. |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend_1)(char) | 뒤에 오는 문자를 모두 제거합니다. |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend_2)(params char[]) | 배열에 지정된 문자 집합의 모든 후행 항목을 제거합니다. |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart)() | 선행 공백 문자를 모두 제거합니다. |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart_1)(char) | 지정된 문자의 선행 항목을 모두 제거합니다. |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart_2)(params char[]) | 배열에 지정된 문자 집합의 선행 항목을 모두 제거합니다. |

### 예

문서에서 모든 텍스트를 가져오는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Text();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "Aspose.one");

// 텍스트 검색
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// 출력 화면에 텍스트 출력
Console.WriteLine(text);
```

페이지에서 모든 텍스트를 가져오는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Text();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "Aspose.one");

// 페이지 노드 목록 가져오기
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // 텍스트 검색
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // 출력 화면에 텍스트 출력
    Console.WriteLine(text);
}
```

글꼴 크기를 늘려 다른 헤더 중에서 페이지의 제목을 강조해 봅시다.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 문서를 Aspose.Note에 로드합니다.
Document document = new Document(dataDir + "Aspose.one");

// 페이지 제목을 반복합니다.
foreach (var title in document.Select(e => e.Title.TitleText))
{
    title.ParagraphStyle.FontSize = 24;
    title.ParagraphStyle.IsBold = true;

    foreach (var run in title.TextRuns)
    {
        run.Style.FontSize = 24;
        run.Style.IsBold = true;
    }
}

document.Save(Path.Combine(dataDir, "ChangePageTitleStyle.pdf"));
```

모든 테이블의 행에서 텍스트를 가져오는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Tables();

// 문서를 Aspose.Note에 로드합니다.
Document document = new Document(dataDir + "Sample1.one");

// 테이블 노드 목록 가져오기
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // 테이블 행을 반복합니다.
    foreach (TableRow row in table)
    {
        // 텍스트 검색
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // 출력 화면에 텍스트 출력
        Console.WriteLine(text);
    }
}
```

테이블에서 텍스트를 가져오는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Tables();

// 문서를 Aspose.Note에 로드합니다.
Document document = new Document(dataDir + "Sample1.one");

// 테이블 노드 목록 가져오기
IList<Table> nodes = document.GetChildNodes<Table>();

// 테이블 수 설정
int tblCount = 0;

foreach (Table table in nodes)
{
    tblCount++;
    Console.WriteLine("table # " + tblCount);

    // 텍스트 검색
    string text = string.Join(Environment.NewLine, table.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

    // 출력 화면에 텍스트 출력
    Console.WriteLine(text);
}
```

강조 표시를 통해 최신 텍스트의 변경 사항을 강조해 봅시다.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 문서를 Aspose.Note에 로드합니다.
Document document = new Document(dataDir + "Aspose.one");

// 지난주에 수정된 RichText 노드를 가져옵니다.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // 강조 색상 설정
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // 강조 색상 설정
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

페이지의 제목을 설정하는 방법을 보여줍니다.

```csharp
string dataDir = RunExamples.GetDataDir_Text();
string outputPath = dataDir + "CreateTitleMsStyle_out.one";

var doc = new Document();
var page = new Page(doc);

page.Title = new Title(doc)
{
    TitleText = new RichText(doc)
    {
        Text = "Title text.",
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleDate = new RichText(doc)
    {
        Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture),
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleTime = new RichText(doc)
    {
        Text = "12:34",
        ParagraphStyle = ParagraphStyle.Default
    }
};

doc.AppendChildLast(page);

doc.Save(outputPath);
```

텍스트의 교정 언어를 설정합니다.

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = ParagraphStyle.Default };
text.Append("United States", new TextStyle() { Language = CultureInfo.GetCultureInfo("en-US") })
    .Append(" Germany", new TextStyle() { Language = CultureInfo.GetCultureInfo("de-DE") })
    .Append(" China", new TextStyle() { Language = CultureInfo.GetCultureInfo("zh-CN") });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetProofingLanguageForText.one"));
```

모든 페이지를 통과하고 텍스트를 교체하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "Aspose.one");

// 모든 RichText 노드 가져오기
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // 도형의 텍스트 바꾸기
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

// 지원되는 파일 형식으로 저장
oneFile.Save(dataDir, SaveFormat.Pdf);
```

단락 스타일을 사용하여 텍스트 형식으로 조작합니다.

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = new ParagraphStyle() { FontName = "Courier New", FontSize = 20 } }
                .Append($"DefaultParagraphFontAndSize{Environment.NewLine}")
                .Append($"OnlyDefaultParagraphFont{Environment.NewLine}", new TextStyle() { FontSize = 14 })
                .Append("OnlyDefaultParagraphFontSize", new TextStyle() { FontName = "Verdana" });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetDefaultParagraphStyle.one"));
```

표의 셀에서 텍스트를 가져오는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Tables();

// 문서를 Aspose.Note에 로드합니다.
Document document = new Document(dataDir + "Sample1.one");

// 테이블 노드 목록 가져오기
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // 테이블 행을 반복합니다.
    foreach (TableRow row in table)
    {
        // TableCell 노드 목록 가져오기
        // 테이블 셀을 통해 반복
        foreach (TableCell cell in row)
        {
            // 텍스트 검색
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // 출력 화면에 텍스트 출력
            Console.WriteLine(text);
        }
    }
}
```

페이지의 텍스트를 통과하고 교체하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// 모든 RichText 노드 가져오기
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // 도형의 텍스트 바꾸기
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// 지원되는 파일 형식으로 저장
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
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

태그가 있는 새 단락을 추가하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Tags();

// Document 클래스의 객체 생성
Document doc = new Document();

// 페이지 클래스 객체 초기화
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 아웃라인 클래스 객체 초기화
Outline outline = new Outline(doc);

// OutlineElement 클래스 객체 초기화
OutlineElement outlineElem = new OutlineElement(doc);
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
RichText text = new RichText(doc) { Text = "OneNote text.", ParagraphStyle = textStyle };
text.Tags.Add(NoteTag.CreateYellowStar());

// 텍스트 노드 추가
outlineElem.AppendChildLast(text);

// 아웃라인 요소 노드 추가
outline.AppendChildLast(outlineElem);

// 아웃라인 노드 추가
page.AppendChildLast(outline);

// 페이지 노드 추가
doc.AppendChildLast(page);

// OneNote 문서 저장
dataDir = dataDir + "AddTextNodeWithTag_out.one";
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

태그 세부 정보에 액세스하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Tags();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "TagFile.one");

// 모든 RichText 노드 가져오기
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// 각 노드를 통해 반복
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // 속성 검색
            Console.WriteLine($"    Completed Time: {noteTag.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTag.CreationTime}");
            Console.WriteLine($"    Font Color: {noteTag.FontColor}");
            Console.WriteLine($"    Status: {noteTag.Status}");
            Console.WriteLine($"    Label: {noteTag.Label}");
            Console.WriteLine($"    Icon: {noteTag.Icon}");
            Console.WriteLine($"    High Light: {noteTag.Highlight}");
        }
    }
}
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

중국어 번호 매기기로 새 목록을 삽입하는 방법을 보여줍니다.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// OneNote 문서 초기화
Aspose.Note.Document doc = new Aspose.Note.Document();

// OneNote 페이지 초기화
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// 텍스트 스타일 설정 적용
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 같은 아웃라인의 숫자는 자동으로 증가합니다.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

//------------------------
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

//------------------------
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

//------------------------
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// OneNote 문서 저장
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

새 글머리 기호 목록을 삽입하는 방법을 보여줍니다.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Document 클래스의 객체 생성
Aspose.Note.Document doc = new Aspose.Note.Document();

// 페이지 클래스 객체 초기화
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 아웃라인 클래스 객체 초기화
Outline outline = new Outline(doc);

// TextStyle 클래스 개체를 초기화하고 서식 지정 속성을 설정합니다.
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// OutlineElement 클래스 개체를 초기화하고 글머리 기호를 적용합니다.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// RichText 클래스 객체 초기화 및 텍스트 스타일 적용
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 아웃라인 요소 추가
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// 아웃라인 노드 추가
page.AppendChildLast(outline);
// 페이지 노드 추가
doc.AppendChildLast(page);

// OneNote 문서 저장
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

번호가 매겨진 새 목록을 삽입하는 방법을 보여줍니다.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Document 클래스의 객체 생성
Document doc = new Document();

// 페이지 클래스 객체 초기화
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 아웃라인 클래스 객체 초기화
Outline outline = new Outline(doc);

// TextStyle 클래스 개체를 초기화하고 서식 지정 속성을 설정합니다.
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// OutlineElement 클래스 객체 초기화 및 번호 매기기 적용
// 같은 아웃라인의 숫자는 자동으로 증가합니다.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 아웃라인 요소 추가
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// 아웃라인 노드 추가
page.AppendChildLast(outline);

// 페이지 노드 추가
doc.AppendChildLast(page);

// OneNote 문서 저장
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

주간 회의를 위한 템플릿을 준비하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Tags();

// Document 클래스의 객체 생성
var headerStyle = new ParagraphStyle() { FontName = "Calibri", FontSize = 16 };
var bodyStyle = new ParagraphStyle() { FontName = "Calibri", FontSize = 12 };

var d = new Document();
bool restartFlag = true;
var outline = d.AppendChildLast(new Page()
                                    {
                                        Title = new Title() { TitleText = new RichText() { Text = $"Weekly meeting {DateTime.Today:d}", ParagraphStyle = ParagraphStyle.Default } }
                                    })
               .AppendChildLast(new Outline() { VerticalOffset = 30, HorizontalOffset = 30 });

outline.AppendChildLast(new OutlineElement())
       .AppendChildLast(new RichText() { Text = "Important", ParagraphStyle = headerStyle });
foreach (var e in new[] { "First", "Second", "Third" })
{
    outline.AppendChildLast(new OutlineElement() { NumberList = CreateListNumberingStyle(bodyStyle, restartFlag) })
           .AppendChildLast(new RichText() { Text = e, ParagraphStyle = bodyStyle });
    restartFlag = false;
}

outline.AppendChildLast(new OutlineElement())
       .AppendChildLast(new RichText() { Text = "TO DO", ParagraphStyle = headerStyle, SpaceBefore = 15 });
restartFlag = true;
foreach (var e in new[] { "First", "Second", "Third" })
{
    outline.AppendChildLast(new OutlineElement() { NumberList = CreateListNumberingStyle(bodyStyle, restartFlag) })
           .AppendChildLast(new RichText() { Text = e, ParagraphStyle = bodyStyle, Tags = { NoteCheckBox.CreateBlueCheckBox() } });
    restartFlag = false;
}

d.Save(Path.Combine(dataDir, "meetingNotes.one"));
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

### 또한보십시오

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [ITaggable](../itaggable/)
* 네임스페이스 [Aspose.Note](../../aspose.note/)
* 집회 [Aspose.Note](../../)


