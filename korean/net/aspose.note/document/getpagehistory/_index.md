---
title: Document.GetPageHistory
second_title: .NET API 참조용 Aspose.Note
description: Document 방법. 가져오기PageHistory 문서에 표시된 각 페이지에 대한 전체 기록을 포함합니다가장 빠른 인덱스 0. 현재 페이지 개정판은 다음과 같이 액세스할 수 있습니다.Current 기록 버전 컬렉션과 별도로 포함됩니다.
type: docs
weight: 100
url: /ko/net/aspose.note/document/getpagehistory/
---
## Document.GetPageHistory method

가져오기[`PageHistory`](../../pagehistory/) 문서에 표시된 각 페이지에 대한 전체 기록을 포함합니다(가장 빠른 인덱스 0). 현재 페이지 개정판은 다음과 같이 액세스할 수 있습니다.[`Current`](../../pagehistory/current/) 기록 버전 컬렉션과 별도로 포함됩니다.

```csharp
public PageHistory GetPageHistory(Page page)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| page | Page | 페이지의 현재 개정판입니다. |

### 반환 값

[`PageHistory`](../../pagehistory/) .

### 예

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

### 또한보십시오

* class [PageHistory](../../pagehistory/)
* class [Page](../../page/)
* class [Document](../)
* 네임스페이스 [Aspose.Note](../../document/)
* 집회 [Aspose.Note](../../../)


