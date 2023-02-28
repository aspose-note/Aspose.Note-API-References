---
title: AttachedFile.Bytes
second_title: .NET API 참조용 Aspose.Note
description: AttachedFile 재산. 포함된 파일의 이진 데이터를 가져옵니다.
type: docs
weight: 50
url: /ko/net/aspose.note/attachedfile/bytes/
---
## AttachedFile.Bytes property

포함된 파일의 이진 데이터를 가져옵니다.

```csharp
public byte[] Bytes { get; }
```

### 예

첨부 파일의 내용을 가져오는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Attachments();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "Sample1.one");

// 첨부 파일 노드 목록 가져오기
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// 모든 노드를 반복합니다.
foreach (AttachedFile file in nodes)
{
    // 첨부 파일을 스트림 객체에 로드
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // 로컬 파일 생성
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // 파일 스트림 복사
            CopyStream(outputStream, fileStream);
        }
    }
}
```

### 또한보십시오

* class [AttachedFile](../)
* 네임스페이스 [Aspose.Note](../../attachedfile/)
* 집회 [Aspose.Note](../../../)


