---
title: Image.LastModifiedTime
second_title: .NET API 참조용 Aspose.Note
description: Image 재산. 마지막 수정 시간을 가져오거나 설정합니다.
type: docs
weight: 130
url: /ko/net/aspose.note/image/lastmodifiedtime/
---
## Image.LastModifiedTime property

마지막 수정 시간을 가져오거나 설정합니다.

```csharp
public DateTime LastModifiedTime { get; set; }
```

### 예

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

### 또한보십시오

* class [Image](../)
* 네임스페이스 [Aspose.Note](../../image/)
* 집회 [Aspose.Note](../../../)


