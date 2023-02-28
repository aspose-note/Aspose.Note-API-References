---
title: Document.FileFormat
second_title: .NET API 참조용 Aspose.Note
description: Document 재산. 파일 형식 가져오기OneNote 2010 OneNote Online.
type: docs
weight: 60
url: /ko/net/aspose.note/document/fileformat/
---
## Document.FileFormat property

파일 형식 가져오기(OneNote 2010, OneNote Online).

```csharp
public FileFormat FileFormat { get; }
```

### 예

문서의 파일 형식을 가져오는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");
switch (document.FileFormat)
{
    case FileFormat.OneNote2010:
        // OneNote 2010 처리
        break;
    case FileFormat.OneNoteOnline:
        // OneNote 온라인 처리
        break;
}
```

### 또한보십시오

* enum [FileFormat](../../fileformat/)
* class [Document](../)
* 네임스페이스 [Aspose.Note](../../document/)
* 집회 [Aspose.Note](../../../)


