---
title: Image.Tags
second_title: Aspose.Note for .NET API リファレンス
description: Image 財産. 段落のすべてのタグのリストを取得します
type: docs
weight: 160
url: /ja/net/aspose.note/image/tags/
---
## Image.Tags property

段落のすべてのタグのリストを取得します。

```csharp
public List<ITag> Tags { get; }
```

### 例

タグ付きの新しい画像を追加する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Tags();

// Document クラスのオブジェクトを作成します
Document doc = new Document();

// Page クラス オブジェクトを初期化します
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline クラス オブジェクトの初期化
Outline outline = new Outline(doc);

// OutlineElement クラス オブジェクトを初期化します
OutlineElement outlineElem = new OutlineElement(doc);

// 画像を読み込む
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

// ドキュメントノードに画像を挿入
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// アウトライン要素ノードを追加
outline.AppendChildLast(outlineElem);

// アウトラインノードを追加
page.AppendChildLast(outline);

// ページノードを追加
doc.AppendChildLast(page);

// OneNote ドキュメントを保存
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
```

### 関連項目

* interface [ITag](../../itag/)
* class [Image](../)
* 名前空間 [Aspose.Note](../../image/)
* 組み立て [Aspose.Note](../../../)


