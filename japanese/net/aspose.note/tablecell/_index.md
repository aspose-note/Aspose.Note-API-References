---
title: Class TableCell
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.TableCell クラス. 表のセルを表します
type: docs
weight: 910
url: /ja/net/aspose.note/tablecell/
---
## TableCell class

表のセルを表します。

```csharp
public sealed class TableCell : CompositeNode<IOutlineChildNode>
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [TableCell](tablecell/#constructor)() | の新しいインスタンスを初期化します`TableCell`class. |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [BackgroundColor](../../aspose.note/tablecell/backgroundcolor/) { get; set; } | 背景色を取得または設定します。 |
| [Document](../../aspose.note/node/document/) { get; } | ノードのドキュメントを取得します。 |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [LastModifiedTime](../../aspose.note/tablecell/lastmodifiedtime/) { get; set; } | 最終変更時刻を取得または設定します。 |
| [MaxWidth](../../aspose.note/tablecell/maxwidth/) { get; } | 最大幅を取得します。 |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | 同じノード ツリー レベルの次のノードを取得します。 |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | ノード タイプを取得します。 |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | 親ノードを取得します。 |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | 同じノード ツリー レベルの前のノードを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| override [Accept](../../aspose.note/tablecell/accept/)(DocumentVisitor) | ノードの訪問者を受け入れます。 |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;IOutlineChildNode&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params IOutlineChildNode[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |

### 例

表のセルからテキストを取得する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Tables();

// ドキュメントを Aspose.Note にロードします。
Document document = new Document(dataDir + "Sample1.one");

// テーブル ノードのリストを取得します
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // 表の行を繰り返します
    foreach (TableRow row in table)
    {
        // TableCell ノードのリストを取得
        // 表のセルを繰り返します
        foreach (TableCell cell in row)
        {
            // テキストを取得
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // 出力画面にテキストを出力
            Console.WriteLine(text);
        }
    }
}
```

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

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* interface [IOutlineChildNode](../ioutlinechildnode/)
* 名前空間 [Aspose.Note](../../aspose.note/)
* 組み立て [Aspose.Note](../../)


