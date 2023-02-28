---
title: Document.IsEncrypted
second_title: .NET API 참조용 Aspose.Note
description: Document 방법. 스트림의 문서가 암호화되었는지 확인합니다. 확인하려면 이 문서를 완전히 로드해야 합니다. 따라서 이 방법은 성능 저하로 이어질 수 있습니다.
type: docs
weight: 150
url: /ko/net/aspose.note/document/isencrypted/
---
## IsEncrypted(Stream, LoadOptions, out Document) {#isencrypted_1}

스트림의 문서가 암호화되었는지 확인합니다. 확인하려면 이 문서를 완전히 로드해야 합니다. 따라서 이 방법은 성능 저하로 이어질 수 있습니다.

```csharp
public static bool IsEncrypted(Stream stream, LoadOptions options, out Document document)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| stream | Stream | 스트림. |
| options | LoadOptions | 로드 옵션입니다. |
| document | Document& | 로드된 문서. |

### 반환 값

문서가 암호화되어 있으면 true를 반환하고 그렇지 않으면 false를 반환합니다.

### 예

문서가 암호로 보호되어 있는지 확인하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

문서가 특정 암호로 암호로 보호되어 있는지 확인하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### 또한보십시오

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* 네임스페이스 [Aspose.Note](../../document/)
* 집회 [Aspose.Note](../../../)

---

## IsEncrypted(Stream, string, out Document) {#isencrypted_2}

스트림의 문서가 암호화되었는지 확인합니다. 확인하려면 이 문서를 완전히 로드해야 합니다. 따라서 이 방법은 성능 저하로 이어질 수 있습니다.

```csharp
public static bool IsEncrypted(Stream stream, string password, out Document document)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| stream | Stream | 스트림. |
| password | String | 문서를 해독하기 위한 암호입니다. |
| document | Document& | 로드된 문서. |

### 반환 값

문서가 암호화되어 있으면 true를 반환하고 그렇지 않으면 false를 반환합니다.

### 예

문서가 암호로 보호되어 있는지 확인하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

문서가 특정 암호로 암호로 보호되어 있는지 확인하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### 또한보십시오

* class [Document](../)
* 네임스페이스 [Aspose.Note](../../document/)
* 집회 [Aspose.Note](../../../)

---

## IsEncrypted(Stream, out Document) {#isencrypted}

스트림의 문서가 암호화되었는지 확인합니다. 확인하려면 이 문서를 완전히 로드해야 합니다. 따라서 이 방법은 성능 저하로 이어질 수 있습니다.

```csharp
public static bool IsEncrypted(Stream stream, out Document document)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| stream | Stream | 스트림. |
| document | Document& | 로드된 문서. |

### 반환 값

문서가 암호화되어 있으면 true를 반환하고 그렇지 않으면 false를 반환합니다.

### 예

문서가 암호로 보호되어 있는지 확인하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

문서가 특정 암호로 암호로 보호되어 있는지 확인하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### 또한보십시오

* class [Document](../)
* 네임스페이스 [Aspose.Note](../../document/)
* 집회 [Aspose.Note](../../../)

---

## IsEncrypted(string, LoadOptions, out Document) {#isencrypted_4}

파일의 문서가 암호화되었는지 확인합니다. 확인하려면 이 문서를 완전히 로드해야 합니다. 따라서 이 방법은 성능 저하로 이어질 수 있습니다.

```csharp
public static bool IsEncrypted(string filePath, LoadOptions options, out Document document)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | String | 파일 경로. |
| options | LoadOptions | 로드 옵션입니다. |
| document | Document& | 로드된 문서. |

### 반환 값

문서가 암호화되어 있으면 true를 반환하고 그렇지 않으면 false를 반환합니다.

### 예

문서가 암호로 보호되어 있는지 확인하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

문서가 특정 암호로 암호로 보호되어 있는지 확인하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### 또한보십시오

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* 네임스페이스 [Aspose.Note](../../document/)
* 집회 [Aspose.Note](../../../)

---

## IsEncrypted(string, out Document) {#isencrypted_3}

파일의 문서가 암호화되었는지 확인합니다. 확인하려면 이 문서를 완전히 로드해야 합니다. 따라서 이 방법은 성능 저하로 이어질 수 있습니다.

```csharp
public static bool IsEncrypted(string filePath, out Document document)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | String | 파일 경로. |
| document | Document& | 로드된 문서. |

### 반환 값

문서가 암호화되어 있으면 true를 반환하고 그렇지 않으면 false를 반환합니다.

### 예

문서가 암호로 보호되어 있는지 확인하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

문서가 특정 암호로 암호로 보호되어 있는지 확인하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### 또한보십시오

* class [Document](../)
* 네임스페이스 [Aspose.Note](../../document/)
* 집회 [Aspose.Note](../../../)

---

## IsEncrypted(string, string, out Document) {#isencrypted_5}

파일의 문서가 암호화되었는지 확인합니다. 확인하려면 이 문서를 완전히 로드해야 합니다. 따라서 이 방법은 성능 저하로 이어질 수 있습니다.

```csharp
public static bool IsEncrypted(string filePath, string password, out Document document)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | String | 파일 경로. |
| password | String | 문서를 해독하기 위한 암호입니다. |
| document | Document& | 로드된 문서. |

### 반환 값

문서가 암호화되어 있으면 true를 반환하고 그렇지 않으면 false를 반환합니다.

### 예

문서가 암호로 보호되어 있는지 확인하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

문서가 특정 암호로 암호로 보호되어 있는지 확인하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### 또한보십시오

* class [Document](../)
* 네임스페이스 [Aspose.Note](../../document/)
* 집회 [Aspose.Note](../../../)


