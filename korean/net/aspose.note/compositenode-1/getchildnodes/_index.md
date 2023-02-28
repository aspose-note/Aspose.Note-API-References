---
title: CompositeNode1.GetChildNodes
second_title: .NET API 참조용 Aspose.Note
description: CompositeNode 방법. 노드 유형별로 모든 하위 노드를 가져옵니다.
type: docs
weight: 70
url: /ko/net/aspose.note/compositenode-1/getchildnodes/
---
## CompositeNode&lt;T&gt;.GetChildNodes&lt;T1&gt; method

노드 유형별로 모든 하위 노드를 가져옵니다.

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

문서에서 이미지를 가져오는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Images();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "Aspose.one");

// 모든 이미지 노드 가져오기
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // 이미지 바이트를 파일에 저장
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

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

* interface [INode](../../inode/)
* class [CompositeNode&lt;T&gt;](../)
* 네임스페이스 [Aspose.Note](../../compositenode-1/)
* 집회 [Aspose.Note](../../../)


