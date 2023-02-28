---
title: Notebook.LoadChildDocument
second_title: Aspose.Note for .NET API リファレンス
description: Notebook 方法. 子ドキュメント ノードを追加します ファイルから既存の OneNote ドキュメントを開きます
type: docs
weight: 120
url: /ja/net/aspose.note/notebook/loadchilddocument/
---
## LoadChildDocument(string) {#loadchilddocument_2}

子ドキュメント ノードを追加します。 ファイルから既存の OneNote ドキュメントを開きます。

```csharp
public void LoadChildDocument(string filePath)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| filePath | String | ファイルパス. |

### 例

ストリームからノートブックを読み込む方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

### 関連項目

* class [Notebook](../)
* 名前空間 [Aspose.Note](../../notebook/)
* 組み立て [Aspose.Note](../../../)

---

## LoadChildDocument(string, LoadOptions) {#loadchilddocument_3}

子ドキュメント ノードを追加します。 ファイルから既存の OneNote ドキュメントを開きます。追加のロード オプションを指定できます。

```csharp
public void LoadChildDocument(string filePath, LoadOptions loadOptions)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| filePath | String | ファイルパス. |
| loadOptions | LoadOptions | ロード オプション。 |

### 関連項目

* class [LoadOptions](../../loadoptions/)
* class [Notebook](../)
* 名前空間 [Aspose.Note](../../notebook/)
* 組み立て [Aspose.Note](../../../)

---

## LoadChildDocument(Stream) {#loadchilddocument}

子ドキュメント ノードを追加します。 ストリームから既存の OneNote ドキュメントを開きます。

```csharp
public void LoadChildDocument(Stream stream)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| stream | Stream | ストリーム. |

### 例

ストリームからノートブックを読み込む方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

### 関連項目

* class [Notebook](../)
* 名前空間 [Aspose.Note](../../notebook/)
* 組み立て [Aspose.Note](../../../)

---

## LoadChildDocument(Stream, LoadOptions) {#loadchilddocument_1}

子ドキュメント ノードを追加します。 ストリームから既存の OneNote ドキュメントを開きます。追加のロード オプションを指定できます。

```csharp
public void LoadChildDocument(Stream stream, LoadOptions loadOptions)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| stream | Stream | ストリーム. |
| loadOptions | LoadOptions | ロード オプション。 |

### 関連項目

* class [LoadOptions](../../loadoptions/)
* class [Notebook](../)
* 名前空間 [Aspose.Note](../../notebook/)
* 組み立て [Aspose.Note](../../../)


