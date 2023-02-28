---
title: Document.IsEncrypted
second_title: Aspose.Note for .NET API 参考
description: Document 方法. 检查流中的文档是否已加密 要检查它我们需要完全加载该文档所以这种方法会导致性能下降
type: docs
weight: 150
url: /zh/net/aspose.note/document/isencrypted/
---
## IsEncrypted(Stream, LoadOptions, out Document) {#isencrypted_1}

检查流中的文档是否已加密。 要检查它，我们需要完全加载该文档。所以这种方法会导致性能下降。

```csharp
public static bool IsEncrypted(Stream stream, LoadOptions options, out Document document)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| stream | Stream | 流. |
| options | LoadOptions | 加载选项。 |
| document | Document& | 加载的文档。 |

### 返回值

如果文档已加密则返回真，否则返回假。

### 例子

显示如何检查文档是否受密码保护。

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

显示如何检查文档是否受特定密码的密码保护。

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

### 也可以看看

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* 命名空间 [Aspose.Note](../../document/)
* 部件 [Aspose.Note](../../../)

---

## IsEncrypted(Stream, string, out Document) {#isencrypted_2}

检查流中的文档是否已加密。 要检查它，我们需要完全加载该文档。所以这种方法会导致性能下降。

```csharp
public static bool IsEncrypted(Stream stream, string password, out Document document)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| stream | Stream | 流. |
| password | String | 解密文档的密码。 |
| document | Document& | 加载的文档。 |

### 返回值

如果文档已加密则返回真，否则返回假。

### 例子

显示如何检查文档是否受密码保护。

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

显示如何检查文档是否受特定密码的密码保护。

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

### 也可以看看

* class [Document](../)
* 命名空间 [Aspose.Note](../../document/)
* 部件 [Aspose.Note](../../../)

---

## IsEncrypted(Stream, out Document) {#isencrypted}

检查流中的文档是否已加密。 要检查它，我们需要完全加载该文档。所以这种方法会导致性能下降。

```csharp
public static bool IsEncrypted(Stream stream, out Document document)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| stream | Stream | 流. |
| document | Document& | 加载的文档。 |

### 返回值

如果文档已加密则返回真，否则返回假。

### 例子

显示如何检查文档是否受密码保护。

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

显示如何检查文档是否受特定密码的密码保护。

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

### 也可以看看

* class [Document](../)
* 命名空间 [Aspose.Note](../../document/)
* 部件 [Aspose.Note](../../../)

---

## IsEncrypted(string, LoadOptions, out Document) {#isencrypted_4}

检查文件中的文档是否已加密。 要检查它，我们需要完全加载该文档。所以这种方法会导致性能下降。

```csharp
public static bool IsEncrypted(string filePath, LoadOptions options, out Document document)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| filePath | String | 文件路径。 |
| options | LoadOptions | 加载选项。 |
| document | Document& | 加载的文档。 |

### 返回值

如果文档已加密则返回真，否则返回假。

### 例子

显示如何检查文档是否受密码保护。

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

显示如何检查文档是否受特定密码的密码保护。

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

### 也可以看看

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* 命名空间 [Aspose.Note](../../document/)
* 部件 [Aspose.Note](../../../)

---

## IsEncrypted(string, out Document) {#isencrypted_3}

检查文件中的文档是否已加密。 要检查它，我们需要完全加载该文档。所以这种方法会导致性能下降。

```csharp
public static bool IsEncrypted(string filePath, out Document document)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| filePath | String | 文件路径。 |
| document | Document& | 加载的文档。 |

### 返回值

如果文档已加密则返回真，否则返回假。

### 例子

显示如何检查文档是否受密码保护。

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

显示如何检查文档是否受特定密码的密码保护。

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

### 也可以看看

* class [Document](../)
* 命名空间 [Aspose.Note](../../document/)
* 部件 [Aspose.Note](../../../)

---

## IsEncrypted(string, string, out Document) {#isencrypted_5}

检查文件中的文档是否已加密。 要检查它，我们需要完全加载该文档。所以这种方法会导致性能下降。

```csharp
public static bool IsEncrypted(string filePath, string password, out Document document)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| filePath | String | 文件路径。 |
| password | String | 解密文档的密码。 |
| document | Document& | 加载的文档。 |

### 返回值

如果文档已加密则返回真，否则返回假。

### 例子

显示如何检查文档是否受密码保护。

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

显示如何检查文档是否受特定密码的密码保护。

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

### 也可以看看

* class [Document](../)
* 命名空间 [Aspose.Note](../../document/)
* 部件 [Aspose.Note](../../../)


