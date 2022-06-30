---
title: IsEncrypted
second_title: Aspose.Note for .NET API Reference
description: Checks whether a document from a stream is encrypted. To check it we need to completely load this document. So this method can lead to performance penalty.
type: docs
weight: 150
url: /net/aspose.note/document/isencrypted/
---
## IsEncrypted(Stream, LoadOptions, out Document) {#isencrypted_1}

Checks whether a document from a stream is encrypted. To check it we need to completely load this document. So this method can lead to performance penalty.

```csharp
public static bool IsEncrypted(Stream stream, LoadOptions options, out Document document)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The stream. |
| options | LoadOptions | The load options. |
| document | Document& | The loaded document. |

### Return Value

Returns true if the document is encrypted otherwise false.

### Examples

Shows how to check if a document is password-protected.

```csharp
// The path to the documents directory.
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

Shows how to check if a document is password-protected by specific password.

```csharp
// The path to the documents directory.
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

### See Also

* class [LoadOptions](../../loadoptions)
* class [Document](../../document)
* namespace [Aspose.Note](../../document)
* assembly [Aspose.Note](../../../)

---

## IsEncrypted(Stream, string, out Document) {#isencrypted_2}

Checks whether a document from a stream is encrypted. To check it we need to completely load this document. So this method can lead to performance penalty.

```csharp
public static bool IsEncrypted(Stream stream, string password, out Document document)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The stream. |
| password | String | The password to decrypt a document. |
| document | Document& | The loaded document. |

### Return Value

Returns true if the document is encrypted otherwise false.

### Examples

Shows how to check if a document is password-protected.

```csharp
// The path to the documents directory.
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

Shows how to check if a document is password-protected by specific password.

```csharp
// The path to the documents directory.
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

### See Also

* class [Document](../../document)
* namespace [Aspose.Note](../../document)
* assembly [Aspose.Note](../../../)

---

## IsEncrypted(Stream, out Document) {#isencrypted}

Checks whether a document from a stream is encrypted. To check it we need to completely load this document. So this method can lead to performance penalty.

```csharp
public static bool IsEncrypted(Stream stream, out Document document)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The stream. |
| document | Document& | The loaded document. |

### Return Value

Returns true if the document is encrypted otherwise false.

### Examples

Shows how to check if a document is password-protected.

```csharp
// The path to the documents directory.
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

Shows how to check if a document is password-protected by specific password.

```csharp
// The path to the documents directory.
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

### See Also

* class [Document](../../document)
* namespace [Aspose.Note](../../document)
* assembly [Aspose.Note](../../../)

---

## IsEncrypted(string, LoadOptions, out Document) {#isencrypted_4}

Checks whether a document from a file is encrypted. To check it we need to completely load this document. So this method can lead to performance penalty.

```csharp
public static bool IsEncrypted(string filePath, LoadOptions options, out Document document)
```

| Parameter | Type | Description |
| --- | --- | --- |
| filePath | String | The file path. |
| options | LoadOptions | The load options. |
| document | Document& | The loaded document. |

### Return Value

Returns true if the document is encrypted otherwise false.

### Examples

Shows how to check if a document is password-protected.

```csharp
// The path to the documents directory.
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

Shows how to check if a document is password-protected by specific password.

```csharp
// The path to the documents directory.
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

### See Also

* class [LoadOptions](../../loadoptions)
* class [Document](../../document)
* namespace [Aspose.Note](../../document)
* assembly [Aspose.Note](../../../)

---

## IsEncrypted(string, out Document) {#isencrypted_3}

Checks whether a document from a file is encrypted. To check it we need to completely load this document. So this method can lead to performance penalty.

```csharp
public static bool IsEncrypted(string filePath, out Document document)
```

| Parameter | Type | Description |
| --- | --- | --- |
| filePath | String | The file path. |
| document | Document& | The loaded document. |

### Return Value

Returns true if the document is encrypted otherwise false.

### Examples

Shows how to check if a document is password-protected.

```csharp
// The path to the documents directory.
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

Shows how to check if a document is password-protected by specific password.

```csharp
// The path to the documents directory.
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

### See Also

* class [Document](../../document)
* namespace [Aspose.Note](../../document)
* assembly [Aspose.Note](../../../)

---

## IsEncrypted(string, string, out Document) {#isencrypted_5}

Checks whether a document from a file is encrypted. To check it we need to completely load this document. So this method can lead to performance penalty.

```csharp
public static bool IsEncrypted(string filePath, string password, out Document document)
```

| Parameter | Type | Description |
| --- | --- | --- |
| filePath | String | The file path. |
| password | String | The password to decrypt a document. |
| document | Document& | The loaded document. |

### Return Value

Returns true if the document is encrypted otherwise false.

### Examples

Shows how to check if a document is password-protected.

```csharp
// The path to the documents directory.
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

Shows how to check if a document is password-protected by specific password.

```csharp
// The path to the documents directory.
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

### See Also

* class [Document](../../document)
* namespace [Aspose.Note](../../document)
* assembly [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
