---
title: Image.OriginalWidth
second_title: .NET API 참조용 Aspose.Note
description: Image 재산. 원래 너비를 가져옵니다. 크기를 조정하기 전 이미지의 원래 너비입니다.
type: docs
weight: 150
url: /ko/net/aspose.note/image/originalwidth/
---
## Image.OriginalWidth property

원래 너비를 가져옵니다. 크기를 조정하기 전 이미지의 원래 너비입니다.

```csharp
public float OriginalWidth { get; }
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


