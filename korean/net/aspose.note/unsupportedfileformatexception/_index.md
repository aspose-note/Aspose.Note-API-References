---
title: Class UnsupportedFileFormatException
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.UnsupportedFileFormatException 수업. 파일 형식이 Aspose.Note. 에서 인식되지 않거나 지원되지 않는 경우 문서 로드 중에 발생합니다.
type: docs
weight: 990
url: /ko/net/aspose.note/unsupportedfileformatexception/
---
## UnsupportedFileFormatException class

파일 형식이 Aspose.Note. 에서 인식되지 않거나 지원되지 않는 경우 문서 로드 중에 발생합니다.

```csharp
public class UnsupportedFileFormatException : Exception
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [FileFormat](../../aspose.note/unsupportedfileformatexception/fileformat/) { get; } | 감지되면 전달된 데이터의 파일 형식을 가져옵니다. |

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


