---
title: Class AttachedFile
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.AttachedFile クラス. 添付ファイルを表します
type: docs
weight: 10
url: /ja/net/aspose.note/attachedfile/
---
## AttachedFile class

添付ファイルを表します。

```csharp
public class AttachedFile : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [AttachedFile](attachedfile/#constructor)() | の新しいインスタンスを初期化します`AttachedFile`class. |
| [AttachedFile](attachedfile/#constructor_6)(string, Stream) | の新しいインスタンスを初期化します`AttachedFile`class. |
| [AttachedFile](attachedfile/#constructor_7)(string, Stream, ImageFormat) | の新しいインスタンスを初期化します`AttachedFile`class. |
| [AttachedFile](attachedfile/#constructor_8)(string, Stream, Stream, ImageFormat) | の新しいインスタンスを初期化します`AttachedFile`class. |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Alignment](../../aspose.note/attachedfile/alignment/) { get; set; } | 配置を取得または設定します。 |
| [AlternativeTextDescription](../../aspose.note/attachedfile/alternativetextdescription/) { get; set; } | 添付ファイルのアイコンの本文と代替テキストを取得または設定します。 |
| [AlternativeTextTitle](../../aspose.note/attachedfile/alternativetexttitle/) { get; set; } | 添付ファイルのアイコンの代替テキストのタイトルを取得または設定します。 |
| [Bytes](../../aspose.note/attachedfile/bytes/) { get; } | 埋め込みファイルのバイナリ データを取得します。 |
| [Document](../../aspose.note/node/document/) { get; } | ノードのドキュメントを取得します。 |
| [Extension](../../aspose.note/attachedfile/extension/) { get; } | 埋め込みファイルの拡張子を取得します。 |
| [FileName](../../aspose.note/attachedfile/filename/) { get; } | 埋め込みファイルの名前を取得します。 |
| [FilePath](../../aspose.note/attachedfile/filepath/) { get; } | 元のファイルへのパスを取得します。 |
| [Height](../../aspose.note/attachedfile/height/) { get; } | 埋め込みファイル アイコンの元の高さを取得します。 |
| [HorizontalOffset](../../aspose.note/attachedfile/horizontaloffset/) { get; set; } | 水平オフセットを取得または設定します。 |
| [Icon](../../aspose.note/attachedfile/icon/) { get; } | 埋め込みファイルに関連付けられているアイコンのバイナリ データを取得します。 |
| [IconExtension](../../aspose.note/attachedfile/iconextension/) { get; } | アイコンの拡張子を取得します。 |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | このノードが複合かどうかを示す値を取得します。 true の場合、ノードは子ノードを持つことができます。 |
| [IsPrintout](../../aspose.note/attachedfile/isprintout/) { get; set; } | ファイルのビューが印刷出力かどうかを示す値を取得または設定します。 |
| [IsSizeSetByUser](../../aspose.note/attachedfile/issizesetbyuser/) { get; set; } | アイコンのサイズの値がユーザーによって明示的に更新されたかどうかを示す値を取得または設定します。 |
| [LastModifiedTime](../../aspose.note/attachedfile/lastmodifiedtime/) { get; set; } | 最終変更時刻を取得または設定します。 |
| [MaxHeight](../../aspose.note/attachedfile/maxheight/) { get; set; } | 埋め込みファイル アイコンを表示する最大の高さを取得または設定します。 |
| [MaxWidth](../../aspose.note/attachedfile/maxwidth/) { get; set; } | 埋め込みファイル アイコンを表示する最大幅を取得または設定します。 |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | 同じノード ツリー レベルの次のノードを取得します。 |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | ノード タイプを取得します。 |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | 親ノードを取得します。 |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | 同じノード ツリー レベルの前のノードを取得します。 |
| [Tags](../../aspose.note/attachedfile/tags/) { get; } | 段落のすべてのタグのリストを取得します。 |
| [Text](../../aspose.note/attachedfile/text/) { get; set; } | 埋め込みファイルのテキスト表現を取得または設定します。文字列には、値 10 (ライン フィード) または 13 (キャリッジ リターン) の文字を含めてはなりません。 |
| [VerticalOffset](../../aspose.note/attachedfile/verticaloffset/) { get; set; } | 垂直オフセットを取得または設定します。 |
| [Width](../../aspose.note/attachedfile/width/) { get; } | 埋め込みファイル アイコンの元の幅を取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| override [Accept](../../aspose.note/attachedfile/accept/)(DocumentVisitor) | ノードの訪問者を受け入れます。 |

### 例

添付ファイルのコンテンツを取得する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Attachments();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Sample1.one");

// 添付ファイル ノードのリストを取得します
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// すべてのノードを繰り返します
foreach (AttachedFile file in nodes)
{
    // ストリームオブジェクトに添付ファイルをロード
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // ローカル ファイルを作成します
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // ファイルストリームをコピー
            CopyStream(outputStream, fileStream);
        }
    }
}
```

filepath を使用してドキュメントにファイルを追加する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Attachments();

// Document クラスのオブジェクトを作成します
Document doc = new Document();

// Page クラス オブジェクトを初期化します
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline クラス オブジェクトの初期化
Outline outline = new Outline(doc);

// OutlineElement クラス オブジェクトを初期化します
OutlineElement outlineElem = new OutlineElement(doc);

// AttachedFile クラス オブジェクトを初期化します
AttachedFile attachedFile = new AttachedFile(doc,  dataDir + "attachment.txt");

// 添付ファイルを追加
outlineElem.AppendChildLast(attachedFile);

// アウトライン要素ノードを追加
outline.AppendChildLast(outlineElem);

// アウトラインノードを追加
page.AppendChildLast(outline);

// ページノードを追加
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileByPath_out.one";
doc.Save(dataDir);
```

ストリームからドキュメントにファイルを追加する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Attachments();

// Document クラスのオブジェクトを作成します
Document doc = new Document();

// Page クラス オブジェクトを初期化します
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline クラス オブジェクトの初期化
Outline outline = new Outline(doc);

// OutlineElement クラス オブジェクトを初期化します
OutlineElement outlineElem = new OutlineElement(doc);

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // AttachedFile クラス オブジェクトを初期化し、そのアイコン パスも渡します
    AttachedFile attachedFile = new AttachedFile(doc, dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // 添付ファイルを追加
    outlineElem.AppendChildLast(attachedFile);
}

// アウトライン要素ノードを追加
outline.AppendChildLast(outlineElem);

// アウトラインノードを追加
page.AppendChildLast(outline);

// ページノードを追加
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileAndSetIcon_out.one";
doc.Save(dataDir);
```

### 関連項目

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [IPageChildNode](../ipagechildnode/)
* interface [ITaggable](../itaggable/)
* 名前空間 [Aspose.Note](../../aspose.note/)
* 組み立て [Aspose.Note](../../)


