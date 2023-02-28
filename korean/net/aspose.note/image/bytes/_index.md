---
title: Image.Bytes
second_title: .NET API 참조용 Aspose.Note
description: Image 재산. 이미지 데이터 저장소를 가져옵니다.
type: docs
weight: 50
url: /ko/net/aspose.note/image/bytes/
---
## Image.Bytes property

이미지 데이터 저장소를 가져옵니다.

```csharp
public byte[] Bytes { get; }
```

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

### 또한보십시오

* class [Image](../)
* 네임스페이스 [Aspose.Note](../../image/)
* 집회 [Aspose.Note](../../../)


