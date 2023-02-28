---
title: Document.Document
second_title: Aspose.Note for .NET API リファレンス
description: Document コンストラクタ. の新しいインスタンスを初期化しますDocument class. 空の OneNote ドキュメントを作成します
type: docs
weight: 10
url: /ja/net/aspose.note/document/document/
---
## Document() {#constructor}

の新しいインスタンスを初期化します[`Document`](../) class. 空の OneNote ドキュメントを作成します。

```csharp
public Document()
```

### 関連項目

* class [Document](../)
* 名前空間 [Aspose.Note](../../document/)
* 組み立て [Aspose.Note](../../../)

---

## Document(string) {#constructor_3}

の新しいインスタンスを初期化します[`Document`](../) class. ファイルから既存の OneNote ドキュメントを開きます。

```csharp
public Document(string filePath)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| filePath | String | ファイルパス. |

### 例外

| 例外 | 調子 |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | ドキュメント形式が認識されていないか、サポートされていません。 |
| [FileCorruptedException](../../filecorruptedexception/) | ドキュメントが壊れている可能性があり、読み込めません。 |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | ドキュメントは暗号化されており、開くにはパスワードが必要ですが、入力したパスワードが正しくありません。 |
| InvalidOperationException | ドキュメントに問題があり、Aspose.Note 開発者に報告する必要があります。 |
| IOException | 入出力例外があります。 |

### 関連項目

* class [Document](../)
* 名前空間 [Aspose.Note](../../document/)
* 組み立て [Aspose.Note](../../../)

---

## Document(string, LoadOptions) {#constructor_4}

の新しいインスタンスを初期化します[`Document`](../)class. ファイルから既存の OneNote ドキュメントを開きます。暗号化パスワードなどの追加オプションを指定できます。

```csharp
public Document(string filePath, LoadOptions loadOptions)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| filePath | String | ファイルパス. |
| loadOptions | LoadOptions | ドキュメントのロードに使用されるオプション。 null にすることができます。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | ドキュメント形式が認識されていないか、サポートされていません。 |
| [FileCorruptedException](../../filecorruptedexception/) | ドキュメントが壊れている可能性があり、読み込めません。 |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | ドキュメントは暗号化されており、開くにはパスワードが必要ですが、入力したパスワードが正しくありません。 |
| InvalidOperationException | ドキュメントに問題があり、Aspose.Note 開発者に報告する必要があります。 |
| IOException | 入出力例外があります。 |

### 関連項目

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* 名前空間 [Aspose.Note](../../document/)
* 組み立て [Aspose.Note](../../../)

---

## Document(Stream) {#constructor_1}

の新しいインスタンスを初期化します[`Document`](../) class. ストリームから既存の OneNote ドキュメントを開きます。

```csharp
public Document(Stream inStream)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| inStream | Stream | ストリーム. |

### 例外

| 例外 | 調子 |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | ドキュメント形式が認識されていないか、サポートされていません。 |
| [FileCorruptedException](../../filecorruptedexception/) | ドキュメントが壊れている可能性があり、読み込めません。 |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | ドキュメントは暗号化されており、開くにはパスワードが必要ですが、入力したパスワードが正しくありません。 |
| InvalidOperationException | ドキュメントに問題があり、Aspose.Note 開発者に報告する必要があります。 |
| IOException | 入出力例外があります。 |
| ArgumentException | ストリームは読み取りをサポートしていないか、null であるか、すでに閉じられています。 |

### 関連項目

* class [Document](../)
* 名前空間 [Aspose.Note](../../document/)
* 組み立て [Aspose.Note](../../../)

---

## Document(Stream, LoadOptions) {#constructor_2}

の新しいインスタンスを初期化します[`Document`](../) class. ストリームから既存の OneNote ドキュメントを開きます。暗号化パスワードなどの追加オプションを指定できます。

```csharp
public Document(Stream inStream, LoadOptions loadOptions)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| inStream | Stream | ストリーム. |
| loadOptions | LoadOptions | ドキュメントのロードに使用されるオプション。 null にすることができます。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | ドキュメント形式が認識されていないか、サポートされていません。 |
| [FileCorruptedException](../../filecorruptedexception/) | ドキュメントが壊れている可能性があり、読み込めません。 |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | ドキュメントは暗号化されており、開くにはパスワードが必要ですが、入力したパスワードが正しくありません。 |
| InvalidOperationException | ドキュメントに問題があり、Aspose.Note 開発者に報告する必要があります。 |
| IOException | 入出力例外があります。 |
| ArgumentException | ストリームは読み取りをサポートしていないか、null であるか、すでに閉じられています。 |

### 関連項目

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* 名前空間 [Aspose.Note](../../document/)
* 組み立て [Aspose.Note](../../../)


