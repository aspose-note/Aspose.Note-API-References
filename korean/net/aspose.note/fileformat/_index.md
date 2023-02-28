---
title: Enum FileFormat
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.FileFormat 열거형. OneNote 파일 형식을 나타냅니다.
type: docs
weight: 90
url: /ko/net/aspose.note/fileformat/
---
## FileFormat enumeration

OneNote 파일 형식을 나타냅니다.

```csharp
public enum FileFormat
```

### 가치

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Unknown | `0` | 알 수 없는 파일 형식입니다. |
| OneNote2007 | `1` | 원노트 2010. |
| OneNote2010 | `2` | 원노트 2010. |
| OneNoteOnline | `3` | OneNote 온라인. |

### 예

OneNote 2007 형식이 지원되지 않아 문서 로드가 실패했는지 확인하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "OneNote2007.one");

try
{
    new Document(fileName);
}
catch (UnsupportedFileFormatException e)
{
    if (e.FileFormat == FileFormat.OneNote2007)
    {
        Console.WriteLine("It looks like the provided file is in OneNote 2007 format that is not supported.");
    }
    else
        throw;
}
```

### 또한보십시오

* 네임스페이스 [Aspose.Note](../../aspose.note/)
* 집회 [Aspose.Note](../../)


