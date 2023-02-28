---
title: Class DocumentVisitor
second_title: Aspose.Note for .NET API 参考
description: Aspose.Note.DocumentVisitor 班级. 以指定节点为根遍历子树的抽象类
type: docs
weight: 70
url: /zh/net/aspose.note/documentvisitor/
---
## DocumentVisitor class

以指定节点为根遍历子树的抽象类。

```csharp
public abstract class DocumentVisitor
```

## 方法

| 姓名 | 描述 |
| --- | --- |
| virtual [VisitAttachedFileEnd](../../aspose.note/documentvisitor/visitattachedfileend/)(AttachedFile) | 结束访问[`AttachedFile`](../attachedfile/)节点. |
| virtual [VisitAttachedFileStart](../../aspose.note/documentvisitor/visitattachedfilestart/)(AttachedFile) | 开始访问[`AttachedFile`](../attachedfile/)节点. |
| virtual [VisitDocumentEnd](../../aspose.note/documentvisitor/visitdocumentend/)(Document) | 结束访问[`Document`](../document/)节点. |
| virtual [VisitDocumentStart](../../aspose.note/documentvisitor/visitdocumentstart/)(Document) | 开始访问[`Document`](../document/)节点. |
| virtual [VisitImageEnd](../../aspose.note/documentvisitor/visitimageend/)(Image) | 结束访问[`Image`](../image/)节点. |
| virtual [VisitImageStart](../../aspose.note/documentvisitor/visitimagestart/)(Image) | 开始访问[`Image`](../image/)节点. |
| virtual [VisitOutlineElementEnd](../../aspose.note/documentvisitor/visitoutlineelementend/)(OutlineElement) | 结束访问[`OutlineElement`](../outlineelement/)节点. |
| virtual [VisitOutlineElementStart](../../aspose.note/documentvisitor/visitoutlineelementstart/)(OutlineElement) | 开始访问[`OutlineElement`](../outlineelement/)节点. |
| virtual [VisitOutlineEnd](../../aspose.note/documentvisitor/visitoutlineend/)(Outline) | 结束访问[`Outline`](../outline/)节点. |
| virtual [VisitOutlineGroupEnd](../../aspose.note/documentvisitor/visitoutlinegroupend/)(OutlineGroup) | 结束访问[`OutlineGroup`](../outlinegroup/)节点. |
| virtual [VisitOutlineGroupStart](../../aspose.note/documentvisitor/visitoutlinegroupstart/)(OutlineGroup) | 开始访问[`OutlineGroup`](../outlinegroup/)节点. |
| virtual [VisitOutlineStart](../../aspose.note/documentvisitor/visitoutlinestart/)(Outline) | 开始访问[`Outline`](../outline/)节点. |
| virtual [VisitPageEnd](../../aspose.note/documentvisitor/visitpageend/)(Page) | 结束访问[`Page`](../page/)节点. |
| virtual [VisitPageStart](../../aspose.note/documentvisitor/visitpagestart/)(Page) | 开始访问[`Page`](../page/)节点. |
| virtual [VisitRichTextEnd](../../aspose.note/documentvisitor/visitrichtextend/)(RichText) | 结束访问[`RichText`](../richtext/)节点. |
| virtual [VisitRichTextStart](../../aspose.note/documentvisitor/visitrichtextstart/)(RichText) | 开始访问[`RichText`](../richtext/)节点. |
| virtual [VisitTableCellEnd](../../aspose.note/documentvisitor/visittablecellend/)(TableCell) | 结束访问[`TableCell`](../tablecell/)节点. |
| virtual [VisitTableCellStart](../../aspose.note/documentvisitor/visittablecellstart/)(TableCell) | 开始访问[`TableCell`](../tablecell/)节点. |
| virtual [VisitTableEnd](../../aspose.note/documentvisitor/visittableend/)(Table) | 结束访问[`Table`](../table/)节点. |
| virtual [VisitTableRowEnd](../../aspose.note/documentvisitor/visittablerowend/)(TableRow) | 结束访问[`TableRow`](../tablerow/)节点. |
| virtual [VisitTableRowStart](../../aspose.note/documentvisitor/visittablerowstart/)(TableRow) | 开始访问[`TableRow`](../tablerow/)节点. |
| virtual [VisitTableStart](../../aspose.note/documentvisitor/visittablestart/)(Table) | 开始访问[`Table`](../table/)节点. |
| virtual [VisitTitleEnd](../../aspose.note/documentvisitor/visittitleend/)(Title) | 结束访问[`Title`](../title/)节点. |
| virtual [VisitTitleStart](../../aspose.note/documentvisitor/visittitlestart/)(Title) | 开始访问[`Title`](../title/)节点. |

### 例子

显示如何使用访问者访问文档的内容。

```csharp
public static void Run()
{
    // 文档目录的路径。
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // 打开我们要转换的文档。
    Document doc = new Document(dataDir + "Aspose.one");

    // 创建一个继承自 DocumentVisitor 类的对象。
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // 这是众所周知的访客模式。让模型接受访客。
    // 模型将通过调用相应的方法来遍历自身
    // 在访问者对象上（这称为访问）。
    //
    // 请注意，对象模型中的每个节点都有 Accept 方法，因此访问
    // 不仅可以对整个文档执行，还可以对文档中的任何节点执行。
    doc.Accept(myConverter);

    // 一旦访问完成，我们就可以检索操作的结果，
    // 在此示例中，已在访问者中积累。
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// 以纯文本格式保存文档的简单实现。作为访客实施。
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
    /// 获取访问者积累的文档的纯文本。
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// 将文本添加到当前输出。尊重启用/禁用的输出标志。
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// 在文档中遇到 RichText 节点时调用。
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// 在文档中遇到文档节点时调用。
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// 在文档中遇到页面节点时调用。
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// 当页面节点的处理完成时调用。
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// 在文档中遇到标题节点时调用。
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// 在文档中遇到图像节点时调用。
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// 在文档中遇到 OutlineGroup 节点时调用。
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// 在文档中遇到大纲节点时调用。
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// 在文档中遇到 OutlineElement 节点时调用。
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// 获取访问者的节点总数
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

### 也可以看看

* 命名空间 [Aspose.Note](../../aspose.note/)
* 部件 [Aspose.Note](../../)


