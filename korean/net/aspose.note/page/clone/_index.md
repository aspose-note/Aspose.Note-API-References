---
title: Page.Clone
second_title: .NET API 참조용 Aspose.Note
description: Page 방법. 페이지를 복제합니다.
type: docs
weight: 140
url: /ko/net/aspose.note/page/clone/
---
## Page.Clone method

페이지를 복제합니다.

```csharp
public Page Clone(bool cloneHistory = false)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| cloneHistory | Boolean | 페이지 기록을 복제해야 하는지 여부를 지정합니다.. |

### 반환 값

페이지 복제본입니다.

### 예

페이지의 현재 버전을 기록에 푸시하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote 문서를 로드하고 첫 번째 자식 가져오기           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.Add(page.Clone());

document.Save(dataDir + "PushCurrentPageVersion_out.one");
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

### 또한보십시오

* class [Page](../)
* 네임스페이스 [Aspose.Note](../../page/)
* 집회 [Aspose.Note](../../../)


