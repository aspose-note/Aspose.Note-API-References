---
title: "Document.Accept"
second_title: "Aspose.Note for .NET API 参考"
description: "Document 方法。接受节点的访问者"
type: docs
weight: 80
url: /zh/net/aspose.note/document/accept/
---
## Document.Accept method

接受节点的访问者。

```csharp
public override void Accept(DocumentVisitor visitor)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| visitor | DocumentVisitor | 从 [`DocumentVisitor`](../../documentvisitor/) 派生的类的对象。 |

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

* class [DocumentVisitor](../../documentvisitor/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)


