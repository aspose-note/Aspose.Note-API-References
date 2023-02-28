---
title: Document.IsEncrypted
second_title: Aspose.Note for .NET API リファレンス
description: Document 方法. ストリームからのドキュメントが暗号化されているかどうかを確認します 確認するにはこのドキュメントを完全にロードする必要がありますしたがってこの方法ではパフォーマンスが低下する可能性があります.
type: docs
weight: 150
url: /ja/net/aspose.note/document/isencrypted/
---
## IsEncrypted(Stream, LoadOptions, out Document) {#isencrypted_1}

ストリームからのドキュメントが暗号化されているかどうかを確認します。 確認するには、このドキュメントを完全にロードする必要があります。したがって、この方法ではパフォーマンスが低下する可能性があります.

```csharp
public static bool IsEncrypted(Stream stream, LoadOptions options, out Document document)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| stream | Stream | ストリーム. |
| options | LoadOptions | ロード オプション。 |
| document | Document& | 読み込まれたドキュメント。 |

### 戻り値

ドキュメントが暗号化されている場合は true、そうでない場合は false を返します。

### 例

ドキュメントがパスワードで保護されているかどうかを確認する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
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

ドキュメントが特定のパスワードによってパスワード保護されているかどうかを確認する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
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

### 関連項目

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* 名前空間 [Aspose.Note](../../document/)
* 組み立て [Aspose.Note](../../../)

---

## IsEncrypted(Stream, string, out Document) {#isencrypted_2}

ストリームからのドキュメントが暗号化されているかどうかを確認します。 確認するには、このドキュメントを完全にロードする必要があります。したがって、この方法ではパフォーマンスが低下する可能性があります.

```csharp
public static bool IsEncrypted(Stream stream, string password, out Document document)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| stream | Stream | ストリーム. |
| password | String | ドキュメントを復号化するためのパスワード。 |
| document | Document& | 読み込まれたドキュメント。 |

### 戻り値

ドキュメントが暗号化されている場合は true、そうでない場合は false を返します。

### 例

ドキュメントがパスワードで保護されているかどうかを確認する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
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

ドキュメントが特定のパスワードによってパスワード保護されているかどうかを確認する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
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

### 関連項目

* class [Document](../)
* 名前空間 [Aspose.Note](../../document/)
* 組み立て [Aspose.Note](../../../)

---

## IsEncrypted(Stream, out Document) {#isencrypted}

ストリームからのドキュメントが暗号化されているかどうかを確認します。 確認するには、このドキュメントを完全にロードする必要があります。したがって、この方法ではパフォーマンスが低下する可能性があります.

```csharp
public static bool IsEncrypted(Stream stream, out Document document)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| stream | Stream | ストリーム. |
| document | Document& | 読み込まれたドキュメント。 |

### 戻り値

ドキュメントが暗号化されている場合は true、そうでない場合は false を返します。

### 例

ドキュメントがパスワードで保護されているかどうかを確認する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
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

ドキュメントが特定のパスワードによってパスワード保護されているかどうかを確認する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
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

### 関連項目

* class [Document](../)
* 名前空間 [Aspose.Note](../../document/)
* 組み立て [Aspose.Note](../../../)

---

## IsEncrypted(string, LoadOptions, out Document) {#isencrypted_4}

ファイルのドキュメントが暗号化されているかどうかをチェックします。 チェックするには、このドキュメントを完全にロードする必要があります。したがって、この方法ではパフォーマンスが低下する可能性があります.

```csharp
public static bool IsEncrypted(string filePath, LoadOptions options, out Document document)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| filePath | String | ファイルパス. |
| options | LoadOptions | ロード オプション。 |
| document | Document& | 読み込まれたドキュメント。 |

### 戻り値

ドキュメントが暗号化されている場合は true、そうでない場合は false を返します。

### 例

ドキュメントがパスワードで保護されているかどうかを確認する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
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

ドキュメントが特定のパスワードによってパスワード保護されているかどうかを確認する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
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

### 関連項目

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* 名前空間 [Aspose.Note](../../document/)
* 組み立て [Aspose.Note](../../../)

---

## IsEncrypted(string, out Document) {#isencrypted_3}

ファイルのドキュメントが暗号化されているかどうかをチェックします。 チェックするには、このドキュメントを完全にロードする必要があります。したがって、この方法ではパフォーマンスが低下する可能性があります.

```csharp
public static bool IsEncrypted(string filePath, out Document document)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| filePath | String | ファイルパス. |
| document | Document& | 読み込まれたドキュメント。 |

### 戻り値

ドキュメントが暗号化されている場合は true、そうでない場合は false を返します。

### 例

ドキュメントがパスワードで保護されているかどうかを確認する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
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

ドキュメントが特定のパスワードによってパスワード保護されているかどうかを確認する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
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

### 関連項目

* class [Document](../)
* 名前空間 [Aspose.Note](../../document/)
* 組み立て [Aspose.Note](../../../)

---

## IsEncrypted(string, string, out Document) {#isencrypted_5}

ファイルのドキュメントが暗号化されているかどうかをチェックします。 チェックするには、このドキュメントを完全にロードする必要があります。したがって、この方法ではパフォーマンスが低下する可能性があります.

```csharp
public static bool IsEncrypted(string filePath, string password, out Document document)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| filePath | String | ファイルパス. |
| password | String | ドキュメントを復号化するためのパスワード。 |
| document | Document& | 読み込まれたドキュメント。 |

### 戻り値

ドキュメントが暗号化されている場合は true、そうでない場合は false を返します。

### 例

ドキュメントがパスワードで保護されているかどうかを確認する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
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

ドキュメントが特定のパスワードによってパスワード保護されているかどうかを確認する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
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

### 関連項目

* class [Document](../)
* 名前空間 [Aspose.Note](../../document/)
* 組み立て [Aspose.Note](../../../)


