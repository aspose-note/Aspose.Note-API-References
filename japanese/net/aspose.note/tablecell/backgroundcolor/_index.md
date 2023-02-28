---
title: TableCell.BackgroundColor
second_title: Aspose.Note for .NET API リファレンス
description: TableCell 財産. 背景色を取得または設定します
type: docs
weight: 20
url: /ja/net/aspose.note/tablecell/backgroundcolor/
---
## TableCell.BackgroundColor property

背景色を取得または設定します。

```csharp
public Color BackgroundColor { get; set; }
```

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

### 関連項目

* class [TableCell](../)
* 名前空間 [Aspose.Note](../../tablecell/)
* 組み立て [Aspose.Note](../../../)


