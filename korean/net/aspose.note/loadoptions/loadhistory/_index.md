---
title: LoadOptions.LoadHistory
second_title: .NET API 참조용 Aspose.Note
description: LoadOptions 재산. 문서 로더가 기록을 무시해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. 이 옵션을 사용하여 메모리 및 CPU 사용량을 줄입니다. 기본값은 다음과 같습니다.진실 .
type: docs
weight: 30
url: /ko/net/aspose.note/loadoptions/loadhistory/
---
## LoadOptions.LoadHistory property

문서 로더가 기록을 무시해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. 이 옵션을 사용하여 메모리 및 CPU 사용량을 줄입니다. 기본값은 다음과 같습니다.`진실` .

```csharp
public bool LoadHistory { get; set; }
```

### 예

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

### 또한보십시오

* class [LoadOptions](../)
* 네임스페이스 [Aspose.Note](../../loadoptions/)
* 집회 [Aspose.Note](../../../)


