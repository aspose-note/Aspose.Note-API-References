---
title: NumberList.FontSize
second_title: .NET API 참조용 Aspose.Note
description: NumberList 재산. 글꼴 크기를 가져오거나 설정합니다.
type: docs
weight: 40
url: /ko/net/aspose.note/numberlist/fontsize/
---
## NumberList.FontSize property

글꼴 크기를 가져오거나 설정합니다.

```csharp
public int FontSize { get; set; }
```

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

### 또한보십시오

* class [NumberList](../)
* 네임스페이스 [Aspose.Note](../../numberlist/)
* 집회 [Aspose.Note](../../../)


