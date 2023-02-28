---
title: Page.GetChildNodes
second_title: Aspose.Note for .NET API リファレンス
description: Page 方法. ノード タイプ別にページのすべての子ノードを取得します
type: docs
weight: 150
url: /ja/net/aspose.note/page/getchildnodes/
---
## Page.GetChildNodes&lt;T1&gt; method

ノード タイプ別にページのすべての子ノードを取得します。

```csharp
public override List<T1> GetChildNodes<T1>()
    where T1 : class, INode
```

| パラメータ | 説明 |
| --- | --- |
| T1 | 返されたリスト内の要素の型。 |

### 戻り値

子ノードのリスト。

### 例

ドキュメントからすべてのテキストを取得する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Text();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Aspose.one");

// テキストを取得
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// 出力画面にテキストを出力
Console.WriteLine(text);
```

ページからすべてのテキストを取得する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Text();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Aspose.one");

// ページノードのリストを取得
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // テキストを取得
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // 出力画面にテキストを出力
    Console.WriteLine(text);
}
```

すべてのページを通過し、テキストを置換する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Aspose.one");

// すべての RichText ノードを取得します
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // 図形のテキストを置き換える
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

// サポートされている任意のファイル形式に保存
oneFile.Save(dataDir, SaveFormat.Pdf);
```

ページのテキストを通過させて置換する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// すべての RichText ノードを取得します
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // 図形のテキストを置き換える
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// サポートされている任意のファイル形式に保存
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

### 関連項目

* interface [INode](../../inode/)
* class [Page](../)
* 名前空間 [Aspose.Note](../../page/)
* 組み立て [Aspose.Note](../../../)


