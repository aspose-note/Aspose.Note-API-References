---
title: Class NumberList
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.NumberList 수업. 번호 매기기 또는 글머리 기호 목록을 나타냅니다.
type: docs
weight: 440
url: /ko/net/aspose.note/numberlist/
---
## NumberList class

번호 매기기 또는 글머리 기호 목록을 나타냅니다.

```csharp
public class NumberList
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [NumberList](numberlist/#constructor_1)(string, string, int) | 의 새 인스턴스를 초기화합니다.`NumberList`class. 이 인스턴스는 글머리 기호 목록을 나타냅니다. |
| [NumberList](numberlist/#constructor)(string, NumberFormat, string, int) | 의 새 인스턴스를 초기화합니다.`NumberList` class. 이 인스턴스는 번호 매기기 목록을 나타냅니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Font](../../aspose.note/numberlist/font/) { get; set; } | 글꼴 이름을 가져오거나 설정합니다. |
| [FontColor](../../aspose.note/numberlist/fontcolor/) { get; set; } | 글꼴 색상을 가져오거나 설정합니다. |
| [FontSize](../../aspose.note/numberlist/fontsize/) { get; set; } | 글꼴 크기를 가져오거나 설정합니다. |
| [Format](../../aspose.note/numberlist/format/) { get; set; } | 라인 헤더의 형식을 가져오거나 설정합니다. 글머리 기호 목록의 경우 글머리 기호 기호를 나타냅니다. |
| [IsBold](../../aspose.note/numberlist/isbold/) { get; set; } | 텍스트 스타일이 굵게 표시되는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [IsItalic](../../aspose.note/numberlist/isitalic/) { get; set; } | 텍스트 스타일이 기울임꼴인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [LastModifiedTime](../../aspose.note/numberlist/lastmodifiedtime/) { get; set; } | 마지막 수정 시간을 가져오거나 설정합니다. |
| [NumberFormat](../../aspose.note/numberlist/numberformat/) { get; set; } | 자동으로 번호가 매겨진 개체 그룹에 사용되는 번호 형식을 가져오거나 설정합니다. 글머리 기호 목록의 경우 null이어야 합니다. |
| [Restart](../../aspose.note/numberlist/restart/) { get; set; } | 목록 항목의 자동 숫자 값을 무시하는 숫자 값을 가져오거나 설정합니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| [Equals](../../aspose.note/numberlist/equals/#equals)(NumberList) | 지정된 개체가 현재 개체와 같은지 여부를 결정합니다. |
| override [Equals](../../aspose.note/numberlist/equals/#equals_1)(object) | 지정된 개체가 현재 개체와 같은지 여부를 결정합니다. |
| override [GetHashCode](../../aspose.note/numberlist/gethashcode/)() | 유형에 대한 해시 함수 역할을 합니다. |
| [GetNumberedListHeader](../../aspose.note/numberlist/getnumberedlistheader/)(int) | 번호가 매겨진 목록 헤더를 가져옵니다. |

### 예

목록 형식에 대한 정보를 검색하는 방법을 보여줍니다.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// 아웃라인 요소의 컬렉션 노드 검색
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// 각 노드를 통해 반복
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // 글꼴 이름 검색
        Console.WriteLine("Font Name: " + list.Font);

        // 폰트 길이 구하기
        Console.WriteLine("Font Length: " + list.Font.Length);

        // 글꼴 크기 검색
        Console.WriteLine("Font Size: " + list.FontSize);

        // 글꼴 색상 검색
        Console.WriteLine("Font Color: " + list.FontColor);

        // 형식 검색
        Console.WriteLine("Font format: " + list.Format);

        // 굵게 확인
        Console.WriteLine("Is bold: " + list.IsBold);

        // 이탤릭체 확인
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
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

### 또한보십시오

* 네임스페이스 [Aspose.Note](../../aspose.note/)
* 집회 [Aspose.Note](../../)


