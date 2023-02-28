---
title: UnsupportedFileFormatException.FileFormat
second_title: .NET API 참조용 Aspose.Note
description: UnsupportedFileFormatException 재산. 감지되면 전달된 데이터의 파일 형식을 가져옵니다.
type: docs
weight: 10
url: /ko/net/aspose.note/unsupportedfileformatexception/fileformat/
---
## UnsupportedFileFormatException.FileFormat property

감지되면 전달된 데이터의 파일 형식을 가져옵니다.

```csharp
public FileFormat FileFormat { get; }
```

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

* enum [FileFormat](../../fileformat/)
* class [UnsupportedFileFormatException](../)
* 네임스페이스 [Aspose.Note](../../unsupportedfileformatexception/)
* 집회 [Aspose.Note](../../../)


