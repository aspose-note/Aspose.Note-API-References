---
title: Class DocumentVisitor
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.DocumentVisitor 수업. 지정된 노드에서 루트가 있는 하위 트리를 통해 반복하기 위한 추상 클래스입니다.
type: docs
weight: 70
url: /ko/net/aspose.note/documentvisitor/
---
## DocumentVisitor class

지정된 노드에서 루트가 있는 하위 트리를 통해 반복하기 위한 추상 클래스입니다.

```csharp
public abstract class DocumentVisitor
```

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| virtual [VisitAttachedFileEnd](../../aspose.note/documentvisitor/visitattachedfileend/)(AttachedFile) | 방문 종료[`AttachedFile`](../attachedfile/) 노드. |
| virtual [VisitAttachedFileStart](../../aspose.note/documentvisitor/visitattachedfilestart/)(AttachedFile) | 방문 시작[`AttachedFile`](../attachedfile/) 노드. |
| virtual [VisitDocumentEnd](../../aspose.note/documentvisitor/visitdocumentend/)(Document) | 방문 종료[`Document`](../document/) 노드. |
| virtual [VisitDocumentStart](../../aspose.note/documentvisitor/visitdocumentstart/)(Document) | 방문 시작[`Document`](../document/) 노드. |
| virtual [VisitImageEnd](../../aspose.note/documentvisitor/visitimageend/)(Image) | 방문 종료[`Image`](../image/) 노드. |
| virtual [VisitImageStart](../../aspose.note/documentvisitor/visitimagestart/)(Image) | 방문 시작[`Image`](../image/) 노드. |
| virtual [VisitOutlineElementEnd](../../aspose.note/documentvisitor/visitoutlineelementend/)(OutlineElement) | 방문 종료[`OutlineElement`](../outlineelement/) 노드. |
| virtual [VisitOutlineElementStart](../../aspose.note/documentvisitor/visitoutlineelementstart/)(OutlineElement) | 방문 시작[`OutlineElement`](../outlineelement/) 노드. |
| virtual [VisitOutlineEnd](../../aspose.note/documentvisitor/visitoutlineend/)(Outline) | 방문 종료[`Outline`](../outline/) 노드. |
| virtual [VisitOutlineGroupEnd](../../aspose.note/documentvisitor/visitoutlinegroupend/)(OutlineGroup) | 방문 종료[`OutlineGroup`](../outlinegroup/) 노드. |
| virtual [VisitOutlineGroupStart](../../aspose.note/documentvisitor/visitoutlinegroupstart/)(OutlineGroup) | 방문 시작[`OutlineGroup`](../outlinegroup/) 노드. |
| virtual [VisitOutlineStart](../../aspose.note/documentvisitor/visitoutlinestart/)(Outline) | 방문 시작[`Outline`](../outline/) 노드. |
| virtual [VisitPageEnd](../../aspose.note/documentvisitor/visitpageend/)(Page) | 방문 종료[`Page`](../page/) 노드. |
| virtual [VisitPageStart](../../aspose.note/documentvisitor/visitpagestart/)(Page) | 방문 시작[`Page`](../page/) 노드. |
| virtual [VisitRichTextEnd](../../aspose.note/documentvisitor/visitrichtextend/)(RichText) | 방문 종료[`RichText`](../richtext/) 노드. |
| virtual [VisitRichTextStart](../../aspose.note/documentvisitor/visitrichtextstart/)(RichText) | 방문 시작[`RichText`](../richtext/) 노드. |
| virtual [VisitTableCellEnd](../../aspose.note/documentvisitor/visittablecellend/)(TableCell) | 방문 종료[`TableCell`](../tablecell/) 노드. |
| virtual [VisitTableCellStart](../../aspose.note/documentvisitor/visittablecellstart/)(TableCell) | 방문 시작[`TableCell`](../tablecell/) 노드. |
| virtual [VisitTableEnd](../../aspose.note/documentvisitor/visittableend/)(Table) | 방문 종료[`Table`](../table/) 노드. |
| virtual [VisitTableRowEnd](../../aspose.note/documentvisitor/visittablerowend/)(TableRow) | 방문 종료[`TableRow`](../tablerow/) 노드. |
| virtual [VisitTableRowStart](../../aspose.note/documentvisitor/visittablerowstart/)(TableRow) | 방문 시작[`TableRow`](../tablerow/) 노드. |
| virtual [VisitTableStart](../../aspose.note/documentvisitor/visittablestart/)(Table) | 방문 시작[`Table`](../table/) 노드. |
| virtual [VisitTitleEnd](../../aspose.note/documentvisitor/visittitleend/)(Title) | 방문 종료[`Title`](../title/) 노드. |
| virtual [VisitTitleStart](../../aspose.note/documentvisitor/visittitlestart/)(Title) | 방문 시작[`Title`](../title/) 노드. |

### 예

방문자를 사용하여 문서의 콘텐츠에 액세스하는 방법을 보여줍니다.

```csharp
public static void Run()
{
    // 문서 디렉토리의 경로.
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // 변환하려는 문서를 엽니다.
    Document doc = new Document(dataDir + "Aspose.one");

    // DocumentVisitor 클래스에서 상속되는 객체를 생성합니다.
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // 이것은 잘 알려진 방문자 패턴입니다. 방문자를 받아들이도록 모델을 가져오십시오.
    // 모델은 해당 메소드를 호출하여 자체적으로 반복합니다.
    // 방문자 개체에 대해(이를 방문이라고 함).
    //
    // 객체 모델의 모든 노드에는 Accept 메서드가 있으므로 방문하는
    // 전체 문서뿐만 아니라 문서의 모든 노드에 대해 실행할 수 있습니다.
    doc.Accept(myConverter);

    // 방문이 완료되면 작업 결과를 검색할 수 있습니다.
    // 이 예에서는 방문자에 누적되었습니다.
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// 일반 텍스트 형식으로 문서를 저장하는 간단한 구현입니다. 방문자로 구현됩니다.
/// </summary>
public class MyOneNoteToTxtWriter : DocumentVisitor
{
    public MyOneNoteToTxtWriter()
    {
        nodecount = 0;
        mIsSkipText = false;
        mBuilder = new StringBuilder();
    }

    /// <summary>
    /// 방문자가 축적한 문서의 일반 텍스트를 가져옵니다.
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// 현재 출력에 텍스트를 추가합니다. 활성화/비활성화 출력 플래그를 존중합니다.
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// RichText 노드가 문서에서 발견될 때 호출됩니다.
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// Document 노드가 문서에서 발견될 때 호출됩니다.
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// 문서에서 페이지 노드를 만나면 호출됩니다.
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// 페이지 노드의 처리가 완료되면 호출됩니다.
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// 문서에서 Title 노드를 만나면 호출됩니다.
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// 문서에서 이미지 노드를 만났을 때 호출됩니다.
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// 문서에서 OutlineGroup 노드를 만나면 호출됩니다.
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// 문서에서 아웃라인 노드를 만나면 호출됩니다.
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// 문서에서 OutlineElement 노드를 만나면 호출됩니다.
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// 방문자의 총 노드 수를 가져옵니다.
    /// </summary>
    public Int32 NodeCount
    {
        get { return this.nodecount; }
    }

    private readonly StringBuilder mBuilder;
    private bool mIsSkipText;
    private Int32 nodecount;
}
```

### 또한보십시오

* 네임스페이스 [Aspose.Note](../../aspose.note/)
* 집회 [Aspose.Note](../../)


