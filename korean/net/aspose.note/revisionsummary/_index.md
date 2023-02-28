---
title: Class RevisionSummary
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.RevisionSummary 수업. 노드 개정에 대한 요약을 나타냅니다.
type: docs
weight: 520
url: /ko/net/aspose.note/revisionsummary/
---
## RevisionSummary class

노드 개정에 대한 요약을 나타냅니다.

```csharp
public class RevisionSummary
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [RevisionSummary](revisionsummary/)() | 기본 생성자입니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [AuthorMostRecent](../../aspose.note/revisionsummary/authormostrecent/) { get; set; } | 가장 최근 작성자를 가져오거나 설정합니다. |
| [LastModifiedTime](../../aspose.note/revisionsummary/lastmodifiedtime/) { get; set; } | 마지막 수정 시간을 가져오거나 설정합니다. |

### 예

페이지의 메타 정보를 편집하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote 문서를 로드하고 첫 번째 자식 가져오기           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

// 이 페이지의 콘텐츠 개정 요약 읽기
var pageRevisionInfo = page.PageContentRevisionSummary;

Console.WriteLine(string.Format(
    "Author:\t{0}\nModified:\t{1}",
    pageRevisionInfo.AuthorMostRecent,
    pageRevisionInfo.LastModifiedTime.ToString("dd.MM.yyyy HH:mm:ss")));

// 이 페이지에 대한 페이지 개정 요약 업데이트
pageRevisionInfo.AuthorMostRecent = "New Author";
pageRevisionInfo.LastModifiedTime = DateTime.Now;

document.Save(dataDir + "WorkingWithPageRevisions_out.one");
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

* 네임스페이스 [Aspose.Note](../../aspose.note/)
* 집회 [Aspose.Note](../../)


