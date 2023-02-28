---
title: Class Notebook
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.Notebook クラス. Aspose.Note ノートブックを表します
type: docs
weight: 410
url: /ja/net/aspose.note/notebook/
---
## Notebook class

Aspose.Note ノートブックを表します。

```csharp
public class Notebook : IEnumerable<INotebookChildNode>, INotebookChildNode
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [Notebook](notebook/#constructor)() | の新しいインスタンスを初期化します`Notebook`class. |
| [Notebook](notebook/#constructor_1)(Stream) | の新しいインスタンスを初期化します`Notebook` class. ストリームから既存の OneNote ノートブックを開きます。 |
| [Notebook](notebook/#constructor_3)(string) | の新しいインスタンスを初期化します`Notebook` class. ファイルから既存の OneNote ノートブックを開きます。 |
| [Notebook](notebook/#constructor_2)(Stream, NotebookLoadOptions) | の新しいインスタンスを初期化します`Notebook` class. ストリームから既存の OneNote ノートブックを開きます。追加の読み込みオプションを指定できます. |
| [Notebook](notebook/#constructor_4)(string, NotebookLoadOptions) | の新しいインスタンスを初期化します`Notebook` class. ファイルから既存の OneNote ノートブックを開きます。子の読み込み戦略 ("lazy"/instant). などの追加オプションを指定できます。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Color](../../aspose.note/notebook/color/) { get; set; } | 色を取得または設定します。 |
| [Count](../../aspose.note/notebook/count/) { get; } | に含まれる要素の数を取得します`Notebook`. |
| [DisplayName](../../aspose.note/notebook/displayname/) { get; set; } | 表示名を取得または設定します。 |
| [FileFormat](../../aspose.note/notebook/fileformat/) { get; } | ファイル形式を取得します (OneNote 2010、OneNote Online). |
| [Guid](../../aspose.note/notebook/guid/) { get; } | オブジェクトのグローバルに一意な ID を取得します。 |
| [IsHistoryEnabled](../../aspose.note/notebook/ishistoryenabled/) { get; set; } | 履歴が有効かどうかを示す値を取得または設定します。 |
| [Item](../../aspose.note/notebook/item/) { get; } | 指定されたインデックスでノートブックの子ノードを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [AppendChild](../../aspose.note/notebook/appendchild/)(INotebookChildNode) | ノードをリストの最後に追加します。 |
| [GetChildNodes&lt;T1&gt;](../../aspose.note/notebook/getchildnodes/)() | ノード タイプ別にすべての子ノードを取得します。 |
| [GetEnumerator](../../aspose.note/notebook/getenumerator/)() | の子ノードを反復処理する列挙子を返します`Notebook`. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument)(Stream) | 子ドキュメント ノードを追加します。 ストリームから既存の OneNote ドキュメントを開きます。 |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument_2)(string) | 子ドキュメント ノードを追加します。 ファイルから既存の OneNote ドキュメントを開きます。 |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument_1)(Stream, LoadOptions) | 子ドキュメント ノードを追加します。 ストリームから既存の OneNote ドキュメントを開きます。追加のロード オプションを指定できます。 |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument_3)(string, LoadOptions) | 子ドキュメント ノードを追加します。 ファイルから既存の OneNote ドキュメントを開きます。追加のロード オプションを指定できます。 |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook)(Stream) | 子ノートブック ノードを追加します。 ストリームから既存の OneNote ノートブックを開きます。 |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook_2)(string) | 子ノートブック ノードを追加します。 ファイルから既存の OneNote ノートブックを開きます。 |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook_1)(Stream, NotebookLoadOptions) | 子ノートブック ノードを追加します。 ストリームから既存の OneNote ノートブックを開きます。追加のロード オプションを指定できます。 |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook_3)(string, NotebookLoadOptions) | 子ノートブック ノードを追加します。 ファイルから既存の OneNote ノートブックを開きます。追加のロード オプションを指定できます。 |
| [RemoveChild](../../aspose.note/notebook/removechild/)(INotebookChildNode) | 子ノードを削除します。 |
| [Save](../../aspose.note/notebook/save/#save)(Stream) | OneNote ドキュメントをストリームに保存します。 |
| [Save](../../aspose.note/notebook/save/#save_3)(string) | OneNote ドキュメントをファイルに保存します。 |
| [Save](../../aspose.note/notebook/save/#save_2)(Stream, NotebookSaveOptions) | 指定された保存オプションを使用して、OneNote ドキュメントをストリームに保存します。 |
| [Save](../../aspose.note/notebook/save/#save_1)(Stream, SaveFormat) | 指定した形式で OneNote ドキュメントをストリームに保存します。 |
| [Save](../../aspose.note/notebook/save/#save_5)(string, NotebookSaveOptions) | 指定された保存オプションを使用して、OneNote ドキュメントをファイルに保存します。 |
| [Save](../../aspose.note/notebook/save/#save_4)(string, SaveFormat) | 指定した形式で OneNote ドキュメントをファイルに保存します。 |

### 例

ノートブックを保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_NoteBook();

var notebook = new Notebook();

dataDir = dataDir + "test_out.onetoc2";

// ノートブックを保存します
notebook.Save(dataDir);
```

ノートブックを PDF 形式で保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote ノートブックを読み込む
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToPDF_out.pdf";

// ノートブックを保存します
notebook.Save(dataDir);
```

ノートブックを画像として保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote ノートブックを読み込む
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToImage_out.png";

// ノートブックを保存します
notebook.Save(dataDir);
```

ノートブックからすべてのテキストを取得する方法を示します。

```csharp
string inputFile = "notebook.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

Notebook rootNotebook = new Notebook(dataDir + inputFile);

IList<RichText> allRichTextNodes = rootNotebook.GetChildNodes<RichText>();
foreach (RichText richTextNode in allRichTextNodes)
{
    Console.WriteLine(richTextNode.Text);
}
```

フラット化されたノートブックを PDF 形式で保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote ノートブックを読み込む
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// ノートブックを保存します
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

それらを遅延ロードするノートブックのドキュメントを反復処理する方法を示します。

```csharp
string inputFile = "Notizbuch öffnen.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

// デフォルトでは、子の読み込みは「遅延」です。
Notebook notebook = new Notebook(dataDir + inputFile);

foreach (var notebookChildNode in notebook.OfType<Document>()) 
{
    // 子ドキュメントの実際のロードはここでのみ発生します。
    // 子ドキュメントで何かをする
}
```

新しいセクションをノートブックに追加する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote ノートブックを読み込む
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Notebook に新しい子を追加します
notebook.AppendChild(new Document(dataDir + "Neuer Abschnitt 1.one"));

dataDir = dataDir + "AddChildNode_out.onetoc2";

// ノートブックを保存します
notebook.Save(dataDir);
```

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

ノートブックを暗号化する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

指定したオプションを使用してノートブックを画像として保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote ノートブックを読み込む
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// ノートブックを保存します
notebook.Save(dataDir, notebookSaveOptions);
```

フラット化されたノートブックを画像として保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote ノートブックを読み込む
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// ノートブックを保存します
notebook.Save(dataDir, notebookSaveOptions);
```

ノートブックからセクションを削除する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote ノートブックを読み込む
var notebook = new Notebook(dataDir + "test.onetoc2");

// その子ノードをトラバースして、目的の子アイテムを検索します
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // ノートブックから子アイテムを削除します
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// ノートブックを保存します
notebook.Save(dataDir);
```

ノートブックのプリロードされたドキュメントを反復処理する方法を示します。

```csharp
// デフォルトでは、子の読み込みは「遅延」です。
// したがって、インスタント ロードが行われたため、
// NotebookLoadOptions.InstantLoading フラグを設定する必要があります。
NotebookLoadOptions loadOptions = new NotebookLoadOptions { InstantLoading = true };

String inputFile = "Notizbuch öffnen.onetoc2";
String dataDir = RunExamples.GetDataDir_NoteBook();
Notebook notebook = new Notebook(dataDir + inputFile, loadOptions);

// すべての子ドキュメントはすでにロードされています。
foreach (INotebookChildNode notebookChildNode in notebook.OfType<Document>()) 
{
   // 子ドキュメントで何かをする
}
```

ノートブックのコンテンツを渡す方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = "Open Notebook.onetoc2";
try
{
    var notebook = new Notebook(dataDir + fileName);
    foreach (var notebookChildNode in notebook)
    {
        Console.WriteLine(notebookChildNode.DisplayName);
        if (notebookChildNode is Document)
        {
            // 子ドキュメントで何かをする
        }
        else if (notebookChildNode is Notebook)
        {
            // 子ノートブックで何かをする
        }
    }
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
```

### 関連項目

* interface [INotebookChildNode](../inotebookchildnode/)
* 名前空間 [Aspose.Note](../../aspose.note/)
* 組み立て [Aspose.Note](../../)


