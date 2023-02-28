---
title: TableColumn.LockedWidth
second_title: .NET API 참조용 Aspose.Note
description: TableColumn 재산. 테이블 열의 너비가 잠겨 있고 테이블 내용에 맞게 자동으로 크기가 조정되지 않는지 여부를 나타내는 값을 가져오거나 설정합니다. 기본적으로 열 너비는 잠겨 있지 않습니다.
type: docs
weight: 20
url: /ko/net/aspose.note/tablecolumn/lockedwidth/
---
## TableColumn.LockedWidth property

테이블 열의 너비가 잠겨 있고 테이블 내용에 맞게 자동으로 크기가 조정되지 않는지 여부를 나타내는 값을 가져오거나 설정합니다. 기본적으로 열 너비는 잠겨 있지 않습니다.

```csharp
public bool LockedWidth { get; set; }
```

### 예

잠긴 열이 있는 테이블을 만드는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Tables();

// Document 클래스의 객체 생성
Document doc = new Document();

// 페이지 클래스 객체 초기화
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// TableRow 클래스 객체 초기화
TableRow row1 = new TableRow(doc);

// TableCell 클래스 객체 초기화 및 텍스트 내용 설정
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
row1.AppendChildLast(cell11);

// TableRow 클래스 객체 초기화
TableRow row2 = new TableRow(doc);

// TableCell 클래스 객체 초기화 및 텍스트 내용 설정
TableCell cell21 = new TableCell(doc);
cell21.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Long   text    with    several   words and    spaces."));
row2.AppendChildLast(cell21);

// 테이블 클래스 객체 초기화
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70, LockedWidth = true } }
              };

// 행 추가
table.AppendChildLast(row1);
table.AppendChildLast(row2);

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// 테이블 노드 추가
outlineElem.AppendChildLast(table);

// 아웃라인 요소 노드 추가
outline.AppendChildLast(outlineElem);

// 아웃라인 노드 추가
page.AppendChildLast(outline);

// 페이지 노드 추가
doc.AppendChildLast(page);
dataDir = dataDir + "CreateTableWithLockedColumns_out.one";
doc.Save(dataDir);
```

### 또한보십시오

* class [TableColumn](../)
* 네임스페이스 [Aspose.Note](../../tablecolumn/)
* 집회 [Aspose.Note](../../../)


