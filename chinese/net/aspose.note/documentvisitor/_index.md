---
title: "DocumentVisitor 类"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.DocumentVisitor 类。用于遍历以指定节点为根的子树的抽象类"
type: docs
weight: 70
url: /zh/net/aspose.note/documentvisitor/
---
## DocumentVisitor class

用于遍历以指定节点为根的子树的抽象类。

```csharp
public abstract class DocumentVisitor
```

## 方法

| 名称 | 描述 |
| --- | --- |
| virtual [VisitAttachedFileEnd](../../aspose.note/documentvisitor/visitattachedfileend/)(AttachedFile) | 结束访问 [`AttachedFile`](../attachedfile/) 节点。 |
| virtual [VisitAttachedFileStart](../../aspose.note/documentvisitor/visitattachedfilestart/)(AttachedFile) | 开始访问 [`AttachedFile`](../attachedfile/) 节点。 |
| virtual [VisitDocumentEnd](../../aspose.note/documentvisitor/visitdocumentend/)(Document) | 结束访问 [`Document`](../document/) 节点。 |
| virtual [VisitDocumentStart](../../aspose.note/documentvisitor/visitdocumentstart/)(Document) | 开始访问 [`Document`](../document/) 节点。 |
| virtual [VisitImageEnd](../../aspose.note/documentvisitor/visitimageend/)(Image) | 结束访问 [`Image`](../image/) 节点。 |
| virtual [VisitImageStart](../../aspose.note/documentvisitor/visitimagestart/)(Image) | 开始访问 [`Image`](../image/) 节点。 |
| virtual [VisitInkDrawingEnd](../../aspose.note/documentvisitor/visitinkdrawingend/)(InkDrawing) | 结束访问 [`InkDrawing`](../inkdrawing/) 节点。 |
| virtual [VisitInkDrawingStart](../../aspose.note/documentvisitor/visitinkdrawingstart/)(InkDrawing) | 开始访问 [`InkDrawing`](../inkdrawing/) 节点。 |
| virtual [VisitInkParagraphEnd](../../aspose.note/documentvisitor/visitinkparagraphend/)(InkParagraph) | 结束访问 [`InkParagraph`](../inkparagraph/) 节点。 |
| virtual [VisitInkParagraphStart](../../aspose.note/documentvisitor/visitinkparagraphstart/)(InkParagraph) | 开始访问 [`InkParagraph`](../inkparagraph/) 节点。 |
| virtual [VisitInkWordEnd](../../aspose.note/documentvisitor/visitinkwordend/)(InkWord) | 结束访问 [`InkWord`](../inkword/) 节点。 |
| virtual [VisitInkWordStart](../../aspose.note/documentvisitor/visitinkwordstart/)(InkWord) | 开始访问 [`InkWord`](../inkword/) 节点。 |
| virtual [VisitLoopEnd](../../aspose.note/documentvisitor/visitloopend/)(Loop) | 结束访问 [`Loop`](../loop/) 节点。 |
| virtual [VisitLoopStart](../../aspose.note/documentvisitor/visitloopstart/)(Loop) | 开始访问 [`Loop`](../loop/) 节点。 |
| virtual [VisitOutlineElementEnd](../../aspose.note/documentvisitor/visitoutlineelementend/)(OutlineElement) | 结束访问 [`OutlineElement`](../outlineelement/) 节点。 |
| virtual [VisitOutlineElementStart](../../aspose.note/documentvisitor/visitoutlineelementstart/)(OutlineElement) | 开始访问 [`OutlineElement`](../outlineelement/) 节点。 |
| virtual [VisitOutlineEnd](../../aspose.note/documentvisitor/visitoutlineend/)(Outline) | 结束访问 [`Outline`](../outline/) 节点。 |
| virtual [VisitOutlineGroupEnd](../../aspose.note/documentvisitor/visitoutlinegroupend/)(OutlineGroup) | 结束访问 [`OutlineGroup`](../outlinegroup/) 节点。 |
| virtual [VisitOutlineGroupStart](../../aspose.note/documentvisitor/visitoutlinegroupstart/)(OutlineGroup) | 开始访问 [`OutlineGroup`](../outlinegroup/) 节点。 |
| virtual [VisitOutlineStart](../../aspose.note/documentvisitor/visitoutlinestart/)(Outline) | 开始访问 [`Outline`](../outline/) 节点。 |
| virtual [VisitPageEnd](../../aspose.note/documentvisitor/visitpageend/)(Page) | 结束访问 [`Page`](../page/) 节点。 |
| virtual [VisitPageStart](../../aspose.note/documentvisitor/visitpagestart/)(Page) | 开始访问 [`Page`](../page/) 节点。 |
| virtual [VisitRichTextEnd](../../aspose.note/documentvisitor/visitrichtextend/)(RichText) | 结束访问 [`RichText`](../richtext/) 节点。 |
| virtual [VisitRichTextStart](../../aspose.note/documentvisitor/visitrichtextstart/)(RichText) | 开始访问 [`RichText`](../richtext/) 节点。 |
| virtual [VisitTableCellEnd](../../aspose.note/documentvisitor/visittablecellend/)(TableCell) | 结束访问 [`TableCell`](../tablecell/) 节点。 |
| virtual [VisitTableCellStart](../../aspose.note/documentvisitor/visittablecellstart/)(TableCell) | 开始访问 [`TableCell`](../tablecell/) 节点。 |
| virtual [VisitTableEnd](../../aspose.note/documentvisitor/visittableend/)(Table) | 结束访问 [`Table`](../table/) 节点。 |
| virtual [VisitTableRowEnd](../../aspose.note/documentvisitor/visittablerowend/)(TableRow) | 结束访问 [`TableRow`](../tablerow/) 节点。 |
| virtual [VisitTableRowStart](../../aspose.note/documentvisitor/visittablerowstart/)(TableRow) | 开始访问 [`TableRow`](../tablerow/) 节点。 |
| virtual [VisitTableStart](../../aspose.note/documentvisitor/visittablestart/)(Table) | 开始访问 [`Table`](../table/) 节点。 |
| virtual [VisitTitleEnd](../../aspose.note/documentvisitor/visittitleend/)(Title) | 结束访问 [`Title`](../title/) 节点。 |
| virtual [VisitTitleStart](../../aspose.note/documentvisitor/visittitlestart/)(Title) | 开始访问 [`Title`](../title/) 节点。 |

## 示例

展示如何使用访问者访问文档的内容。

```csharp
public static void Run()
{
    // 文档目录的路径。
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // 打开我们想要转换的文档。
    Document doc = new Document(dataDir + "Aspose.one");

    // 创建一个继承自 DocumentVisitor 类的对象。
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // 这是众所周知的 Visitor 模式。让模型接受访问者。
    // 模型将通过调用相应的方法自行遍历
    // 在访问者对象上（这称为访问）。
    //
    // 请注意，对象模型中的每个节点都有 Accept 方法，因此访问
    // 不仅可以对整个文档执行，也可以对文档中的任何节点执行。
    doc.Accept(myConverter);

    // 一旦访问完成，我们可以检索操作的结果，
    // 在本例中，该结果已在访问者中累积。
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// 简单实现将文档保存为纯文本格式。实现为 Visitor。
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
    /// 获取由访问者累积的文档纯文本。
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// 向当前输出添加文本。遵守已启用/已禁用的输出标志。
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// 当文档中遇到 RichText 节点时调用。
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// 当文档中遇到 Document 节点时调用。
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// 当文档中遇到 Page 节点时调用。
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// 当 Page 节点的处理完成时调用。
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// 当文档中遇到 Title 节点时调用。
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// 当文档中遇到 Image 节点时调用。
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// 当文档中遇到 OutlineGroup 节点时调用。
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// 当文档中遇到 Outline 节点时调用。
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// 当文档中遇到 OutlineElement 节点时调用。
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// 获取 Visitor 的节点总数
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

### 另请参阅

* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


