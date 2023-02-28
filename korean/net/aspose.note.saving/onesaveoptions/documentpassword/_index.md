---
title: OneSaveOptions.DocumentPassword
second_title: .NET API 참조용 Aspose.Note
description: OneSaveOptions 재산. 문서 내용을 암호화하기 위한 암호를 가져오거나 설정합니다.
type: docs
weight: 20
url: /ko/net/aspose.note.saving/onesaveoptions/documentpassword/
---
## OneSaveOptions.DocumentPassword property

문서 내용을 암호화하기 위한 암호를 가져오거나 설정합니다.

```csharp
public string DocumentPassword { get; set; }
```

### 예

암호화로 문서를 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

### 또한보십시오

* class [OneSaveOptions](../)
* 네임스페이스 [Aspose.Note.Saving](../../onesaveoptions/)
* 집회 [Aspose.Note](../../../)


