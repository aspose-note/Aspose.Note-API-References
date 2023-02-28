---
title: TableCell.BackgroundColor
second_title: .NET API 참조용 Aspose.Note
description: TableCell 재산. 배경색을 가져오거나 설정합니다.
type: docs
weight: 20
url: /ko/net/aspose.note/tablecell/backgroundcolor/
---
## TableCell.BackgroundColor property

배경색을 가져오거나 설정합니다.

```csharp
public Color BackgroundColor { get; set; }
```

### 예

셀의 배경색을 설정하는 방법을 보여줍니다.

```csharp
// Document 클래스의 객체 생성
Document doc = new Document();

// TableCell 클래스 객체 초기화 및 텍스트 내용 설정
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
cell11.BackgroundColor = Color.Coral;

// TableRow 클래스 객체 초기화
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

// 페이지 클래스 객체 초기화
Page page = new Page(doc);
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

### 또한보십시오

* class [TableCell](../)
* 네임스페이스 [Aspose.Note](../../tablecell/)
* 집회 [Aspose.Note](../../../)


