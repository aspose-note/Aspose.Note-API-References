---
title: Page.GetChildNodes
second_title: .NET API 참조용 Aspose.Note
description: Page 방법. 노드 유형별로 페이지의 모든 자식 노드를 가져옵니다.
type: docs
weight: 150
url: /ko/net/aspose.note/page/getchildnodes/
---
## Page.GetChildNodes&lt;T1&gt; method

노드 유형별로 페이지의 모든 자식 노드를 가져옵니다.

```csharp
public override List<T1> GetChildNodes<T1>()
    where T1 : class, INode
```

| 모수 | 설명 |
| --- | --- |
| T1 | 반환된 목록의 요소 유형입니다. |

### 반환 값

자식 노드 목록입니다.

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

### 또한보십시오

* interface [INode](../../inode/)
* class [Page](../)
* 네임스페이스 [Aspose.Note](../../page/)
* 집회 [Aspose.Note](../../../)


