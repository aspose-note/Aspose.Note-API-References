---
title: Page.IsConflictPage
second_title: .NET API 참조용 Aspose.Note
description: Page 재산. 이 페이지가 충돌 페이지인지 여부를 나타내는 값을 가져오거나 설정합니다.
type: docs
weight: 50
url: /ko/net/aspose.note/page/isconflictpage/
---
## Page.IsConflictPage property

이 페이지가 충돌 페이지인지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool IsConflictPage { get; set; }
```

### 비고

두 명의 사용자가 동일한 콘텐츠를 업데이트하려고 하면 충돌 페이지가 발생합니다. 이 경우 첫 번째 사용자의 변경 사항은 평소와 같이 기록됩니다. 다른 사용자의 변경 사항은 병합할 수 없습니다. 따라서 페이지 복사본만 생성됩니다. 충돌로 표시됩니다.

이 버전에서 충돌은 첫 번째 사용자의 변경 사항을 위해 해결됩니다. 따라서 문서에 충돌 페이지가 있으면 기록에 표시되지만 저장 시 건너뜁니다. 이 페이지를 저장하려면 이 플래그를 재설정할 수 있습니다. 평소와 같이 역사상.

충돌 페이지 조작에 대한 자세한 샘플은 온라인 문서에서 찾을 수 있습니다.

### 예

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

* class [Page](../)
* 네임스페이스 [Aspose.Note](../../page/)
* 집회 [Aspose.Note](../../../)


