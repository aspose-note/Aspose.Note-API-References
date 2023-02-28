---
title: TableColumn.LockedWidth
second_title: Aspose.Note for .NET API リファレンス
description: TableColumn 財産. テーブルの列の幅がロックされておりテーブルの内容に合わせて自動的にサイズ変更されないかどうかを示す値を取得または設定します. デフォルトでは列の幅はロックされていません.
type: docs
weight: 20
url: /ja/net/aspose.note/tablecolumn/lockedwidth/
---
## TableColumn.LockedWidth property

テーブルの列の幅がロックされており、テーブルの内容に合わせて自動的にサイズ変更されないかどうかを示す値を取得または設定します. デフォルトでは、列の幅はロックされていません.

```csharp
public bool LockedWidth { get; set; }
```

### 例

ロックされた列を含むテーブルを作成する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Tables();

// Document クラスのオブジェクトを作成します
Document doc = new Document();

// Page クラス オブジェクトを初期化します
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// TableRow クラス オブジェクトを初期化します
TableRow row1 = new TableRow(doc);

// TableCell クラス オブジェクトを初期化し、テキスト コンテンツを設定します
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
row1.AppendChildLast(cell11);

// TableRow クラス オブジェクトを初期化します
TableRow row2 = new TableRow(doc);

// TableCell クラス オブジェクトを初期化し、テキスト コンテンツを設定します
TableCell cell21 = new TableCell(doc);
cell21.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Long   text    with    several   words and    spaces."));
row2.AppendChildLast(cell21);

// Table クラス オブジェクトを初期化します
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70, LockedWidth = true } }
              };

// 行を追加
table.AppendChildLast(row1);
table.AppendChildLast(row2);

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// テーブルノードを追加
outlineElem.AppendChildLast(table);

// アウトライン要素ノードを追加
outline.AppendChildLast(outlineElem);

// アウトラインノードを追加
page.AppendChildLast(outline);

// ページノードを追加
doc.AppendChildLast(page);
dataDir = dataDir + "CreateTableWithLockedColumns_out.one";
doc.Save(dataDir);
```

### 関連項目

* class [TableColumn](../)
* 名前空間 [Aspose.Note](../../tablecolumn/)
* 組み立て [Aspose.Note](../../../)


