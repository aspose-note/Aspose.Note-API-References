---
title: "Document.IsEncrypted"
second_title: "Aspose.Note for .NET API 参考"
description: "Document 方法。检查来自流的文档是否已加密。要进行检查，需要完全加载此文档。因此此方法可能导致性能损失"
type: docs
weight: 150
url: /zh/net/aspose.note/document/isencrypted/
---
## IsEncrypted(Stream, LoadOptions, out Document) {#isencrypted_1}

检查来自流的文档是否已加密。要进行检查，需要完整加载该文档。因此此方法可能导致性能损失。

```csharp
public static bool IsEncrypted(Stream stream, LoadOptions options, out Document document)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | 流。 |
| 选项 | LoadOptions | 加载选项。 |
| 文档 | Document& | 已加载的文档。 |

### 返回值

如果文档已加密则返回 true，否则返回 false。

## 示例

展示如何检查文档是否受密码保护。

```csharp
// 文档目录的路径。
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

展示如何检查文档是否被特定密码保护。

```csharp
// 文档目录的路径。
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

### 另请参阅

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## IsEncrypted(Stream, string, out Document) {#isencrypted_2}

检查来自流的文档是否已加密。要进行检查，需要完整加载该文档。因此此方法可能导致性能损失。

```csharp
public static bool IsEncrypted(Stream stream, string password, out Document document)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | 流。 |
| 密码 | String | 用于解密文档的密码。 |
| 文档 | Document& | 已加载的文档。 |

### 返回值

如果文档已加密则返回 true，否则返回 false。

## 示例

展示如何检查文档是否受密码保护。

```csharp
// 文档目录的路径。
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

展示如何检查文档是否被特定密码保护。

```csharp
// 文档目录的路径。
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

### 另请参阅

* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## IsEncrypted(Stream, out Document) {#isencrypted}

检查来自流的文档是否已加密。要进行检查，需要完整加载该文档。因此此方法可能导致性能损失。

```csharp
public static bool IsEncrypted(Stream stream, out Document document)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | 流。 |
| 文档 | Document& | 已加载的文档。 |

### 返回值

如果文档已加密则返回 true，否则返回 false。

## 示例

展示如何检查文档是否受密码保护。

```csharp
// 文档目录的路径。
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

展示如何检查文档是否被特定密码保护。

```csharp
// 文档目录的路径。
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

### 另请参阅

* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## IsEncrypted(string, LoadOptions, out Document) {#isencrypted_4}

检查来自文件的文档是否已加密。要进行检查，需要完整加载该文档。因此此方法可能导致性能损失。

```csharp
public static bool IsEncrypted(string filePath, LoadOptions options, out Document document)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filePath | String | 文件路径。 |
| 选项 | LoadOptions | 加载选项。 |
| 文档 | Document& | 已加载的文档。 |

### 返回值

如果文档已加密则返回 true，否则返回 false。

## 示例

展示如何检查文档是否受密码保护。

```csharp
// 文档目录的路径。
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

展示如何检查文档是否被特定密码保护。

```csharp
// 文档目录的路径。
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

### 另请参阅

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## IsEncrypted(string, out Document) {#isencrypted_3}

检查来自文件的文档是否已加密。要进行检查，需要完整加载该文档。因此此方法可能导致性能损失。

```csharp
public static bool IsEncrypted(string filePath, out Document document)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filePath | String | 文件路径。 |
| 文档 | Document& | 已加载的文档。 |

### 返回值

如果文档已加密则返回 true，否则返回 false。

## 示例

展示如何检查文档是否受密码保护。

```csharp
// 文档目录的路径。
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

展示如何检查文档是否被特定密码保护。

```csharp
// 文档目录的路径。
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

### 另请参阅

* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## IsEncrypted(string, string, out Document) {#isencrypted_5}

检查来自文件的文档是否已加密。要进行检查，需要完整加载该文档。因此此方法可能导致性能损失。

```csharp
public static bool IsEncrypted(string filePath, string password, out Document document)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filePath | String | 文件路径。 |
| 密码 | String | 用于解密文档的密码。 |
| 文档 | Document& | 已加载的文档。 |

### 返回值

如果文档已加密则返回 true，否则返回 false。

## 示例

展示如何检查文档是否受密码保护。

```csharp
// 文档目录的路径。
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

展示如何检查文档是否被特定密码保护。

```csharp
// 文档目录的路径。
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

### 另请参阅

* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)


