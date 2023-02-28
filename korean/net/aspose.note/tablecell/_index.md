---
title: Class TableCell
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.TableCell 수업. 테이블 셀을 나타냅니다.
type: docs
weight: 910
url: /ko/net/aspose.note/tablecell/
---
## TableCell class

테이블 셀을 나타냅니다.

```csharp
public sealed class TableCell : CompositeNode<IOutlineChildNode>
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [TableCell](tablecell/#constructor)() | 의 새 인스턴스를 초기화합니다.`TableCell` 클래스. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [BackgroundColor](../../aspose.note/tablecell/backgroundcolor/) { get; set; } | 배경색을 가져오거나 설정합니다. |
| [Document](../../aspose.note/node/document/) { get; } | 노드의 문서를 가져옵니다. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [LastModifiedTime](../../aspose.note/tablecell/lastmodifiedtime/) { get; set; } | 마지막 수정 시간을 가져오거나 설정합니다. |
| [MaxWidth](../../aspose.note/tablecell/maxwidth/) { get; } | 최대 너비를 가져옵니다. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | 동일한 노드 트리 수준에서 다음 노드를 가져옵니다. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | 노드 유형을 가져옵니다. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | 상위 노드를 가져옵니다. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | 동일한 노드 트리 수준에서 이전 노드를 가져옵니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| override [Accept](../../aspose.note/tablecell/accept/)(DocumentVisitor) | 노드의 방문자를 수락합니다. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;IOutlineChildNode&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params IOutlineChildNode[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |

### 예

표의 셀에서 텍스트를 가져오는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Tables();

// 문서를 Aspose.Note에 로드합니다.
Document document = new Document(dataDir + "Sample1.one");

// 테이블 노드 목록 가져오기
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // 테이블 행을 반복합니다.
    foreach (TableRow row in table)
    {
        // TableCell 노드 목록 가져오기
        // 테이블 셀을 통해 반복
        foreach (TableCell cell in row)
        {
            // 텍스트 검색
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // 출력 화면에 텍스트 출력
            Console.WriteLine(text);
        }
    }
}
```

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

태그로 새 테이블을 추가하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Tags();

// Document 클래스의 객체 생성
Document doc = new Document();

// 페이지 클래스 객체 초기화
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// TableRow 클래스 객체 초기화
TableRow row = new TableRow(doc);

// TableCell 클래스 객체 초기화
TableCell cell = new TableCell(doc);

// 셀 내용 삽입
cell.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Single cell."));

// 행 노드에 셀 추가
row.AppendChildLast(cell);

// 테이블 노드 초기화
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70 } }
              };

// 테이블에 행 노드 삽입
table.AppendChildLast(row);

// 이 테이블 노드에 태그 추가
table.Tags.Add(NoteTag.CreateQuestionMark());

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// 테이블 노드 추가
outlineElem.AppendChildLast(table);

// 아웃라인 요소 추가
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// OneNote 문서 저장
dataDir = dataDir + "AddTableNodeWithTag_out.one";
doc.Save(dataDir);
```

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

새 테이블을 만드는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Tables();

// Document 클래스의 객체 생성
Document doc = new Document();

// 페이지 클래스 객체 초기화
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// TableRow 클래스 객체 초기화
TableRow row1 = new TableRow(doc);

// TableCell 클래스 객체 초기화
TableCell cell11 = new TableCell(doc);
TableCell cell12 = new TableCell(doc);
TableCell cell13 = new TableCell(doc);

// 테이블 셀에 아웃라인 요소 추가
cell11.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.1"));
cell12.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.2"));
cell13.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.3"));

// 테이블 셀을 행으로
row1.AppendChildLast(cell11);
row1.AppendChildLast(cell12);
row1.AppendChildLast(cell13);

// TableRow 클래스 객체 초기화
TableRow row2 = new TableRow(doc);

// TableCell 클래스 객체 초기화
TableCell cell21 = new TableCell(doc);
TableCell cell22 = new TableCell(doc);
TableCell cell23 = new TableCell(doc);

// 테이블 셀에 아웃라인 요소 추가
cell21.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.1"));
cell22.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.2"));
cell23.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.3"));

// 테이블 셀을 행에 추가
row2.AppendChildLast(cell21);
row2.AppendChildLast(cell22);
row2.AppendChildLast(cell23);

// Table 클래스 객체 초기화 및 열 너비 설정
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 200 }, new TableColumn { Width = 200 }, new TableColumn { Width = 200 } }
              };

// 테이블 행을 테이블에 추가
table.AppendChildLast(row1);
table.AppendChildLast(row2);

// 아웃라인 객체 초기화
Outline outline = new Outline(doc);

// OutlineElement 객체 초기화
OutlineElement outlineElem = new OutlineElement(doc);

// 아웃라인 요소 노드에 테이블 추가
outlineElem.AppendChildLast(table);

// 외곽선에 외곽선 요소 추가
outline.AppendChildLast(outlineElem);

// 페이지 노드에 아웃라인 추가
page.AppendChildLast(outline);

// 문서 노드에 페이지 추가
doc.AppendChildLast(page);
dataDir = dataDir + "InsertTable_out.one";
doc.Save(dataDir);
```

### 또한보십시오

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* interface [IOutlineChildNode](../ioutlinechildnode/)
* 네임스페이스 [Aspose.Note](../../aspose.note/)
* 집회 [Aspose.Note](../../)


