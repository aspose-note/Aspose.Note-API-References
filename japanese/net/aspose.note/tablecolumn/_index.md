---
title: Class TableColumn
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.TableColumn クラス. テーブル列を表します
type: docs
weight: 920
url: /ja/net/aspose.note/tablecolumn/
---
## TableColumn class

テーブル列を表します。

```csharp
public sealed class TableColumn
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [TableColumn](tablecolumn/)() | デフォルトのコンストラクター。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [LockedWidth](../../aspose.note/tablecolumn/lockedwidth/) { get; set; } | テーブルの列の幅がロックされており、テーブルの内容に合わせて自動的にサイズ変更されないかどうかを示す値を取得または設定します. デフォルトでは、列の幅はロックされていません. |
| [Width](../../aspose.note/tablecolumn/width/) { get; set; } | 幅を取得または設定します。 |

### 例

セルの背景色を設定する方法を示します。

```csharp
// Document クラスのオブジェクトを作成します
Document doc = new Document();

// TableCell クラス オブジェクトを初期化し、テキスト コンテンツを設定します
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
cell11.BackgroundColor = Color.Coral;

// TableRow クラス オブジェクトを初期化します
TableRow row = new TableRow(doc);
row.AppendChildLast(cell11);

Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn() { Width = 200 } }
              };
table.AppendChildLast(row);

OutlineElement oe = new OutlineElement(doc);
oe.AppendChildLast(table);

Outline o = new Outline(doc);
o.AppendChildLast(oe);

// Page クラス オブジェクトを初期化します
Page page = new Page(doc);
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

タグを使用して新しいテーブルを追加する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Tags();

// Document クラスのオブジェクトを作成します
Document doc = new Document();

// Page クラス オブジェクトを初期化します
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// TableRow クラス オブジェクトを初期化します
TableRow row = new TableRow(doc);

// TableCell クラス オブジェクトを初期化します
TableCell cell = new TableCell(doc);

// セルの内容を挿入
cell.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Single cell."));

// 行ノードにセルを追加
row.AppendChildLast(cell);

// テーブルノードを初期化
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70 } }
              };

// テーブルに行ノードを挿入
table.AppendChildLast(row);

// このテーブル ノードにタグを追加します
table.Tags.Add(NoteTag.CreateQuestionMark());

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// テーブルノードを追加
outlineElem.AppendChildLast(table);

// アウトライン要素を追加
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// OneNote ドキュメントを保存
dataDir = dataDir + "AddTableNodeWithTag_out.one";
doc.Save(dataDir);
```

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

新しいテーブルを作成する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Tables();

// Document クラスのオブジェクトを作成します
Document doc = new Document();

// Page クラス オブジェクトを初期化します
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// TableRow クラス オブジェクトを初期化します
TableRow row1 = new TableRow(doc);

// TableCell クラス オブジェクトを初期化します
TableCell cell11 = new TableCell(doc);
TableCell cell12 = new TableCell(doc);
TableCell cell13 = new TableCell(doc);

// 表のセルにアウトライン要素を追加します
cell11.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.1"));
cell12.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.2"));
cell13.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.3"));

// 表のセルを行に
row1.AppendChildLast(cell11);
row1.AppendChildLast(cell12);
row1.AppendChildLast(cell13);

// TableRow クラス オブジェクトを初期化します
TableRow row2 = new TableRow(doc);

// TableCell クラス オブジェクトを初期化します
TableCell cell21 = new TableCell(doc);
TableCell cell22 = new TableCell(doc);
TableCell cell23 = new TableCell(doc);

// 表のセルにアウトライン要素を追加します
cell21.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.1"));
cell22.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.2"));
cell23.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.3"));

// 表のセルを行に追加します
row2.AppendChildLast(cell21);
row2.AppendChildLast(cell22);
row2.AppendChildLast(cell23);

// Table クラス オブジェクトを初期化し、列幅を設定します
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 200 }, new TableColumn { Width = 200 }, new TableColumn { Width = 200 } }
              };

// テーブル行をテーブルに追加
table.AppendChildLast(row1);
table.AppendChildLast(row2);

// Outline オブジェクトを初期化します
Outline outline = new Outline(doc);

// OutlineElement オブジェクトを初期化します
OutlineElement outlineElem = new OutlineElement(doc);

// アウトライン要素ノードにテーブルを追加
outlineElem.AppendChildLast(table);

// アウトライン要素をアウトラインに追加
outline.AppendChildLast(outlineElem);

// ページノードにアウトラインを追加
page.AppendChildLast(outline);

// ドキュメントノードにページを追加
doc.AppendChildLast(page);
dataDir = dataDir + "InsertTable_out.one";
doc.Save(dataDir);
```

### 関連項目

* 名前空間 [Aspose.Note](../../aspose.note/)
* 組み立て [Aspose.Note](../../)


