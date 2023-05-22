---
title: Class DocumentVisitor
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.DocumentVisitor class. The abstract class for iterating through subtree with root at the specified node
type: docs
weight: 40
url: /net/aspose.note/documentvisitor/
---
## DocumentVisitor class

The abstract class for iterating through subtree with root at the specified node.

```csharp
public abstract class DocumentVisitor
```

## Methods

| Name | Description |
| --- | --- |
| virtual [VisitAttachedFileEnd](../../aspose.note/documentvisitor/visitattachedfileend/)(AttachedFile) | End to visit the [`AttachedFile`](../attachedfile/) node. |
| virtual [VisitAttachedFileStart](../../aspose.note/documentvisitor/visitattachedfilestart/)(AttachedFile) | Start to visit the [`AttachedFile`](../attachedfile/) node. |
| virtual [VisitDocumentEnd](../../aspose.note/documentvisitor/visitdocumentend/)(Document) | End to visit the [`Document`](../document/) node. |
| virtual [VisitDocumentStart](../../aspose.note/documentvisitor/visitdocumentstart/)(Document) | Start to visit the [`Document`](../document/) node. |
| virtual [VisitImageEnd](../../aspose.note/documentvisitor/visitimageend/)(Image) | End to visit the [`Image`](../image/) node. |
| virtual [VisitImageStart](../../aspose.note/documentvisitor/visitimagestart/)(Image) | Start to visit the [`Image`](../image/) node. |
| virtual [VisitInkDrawingEnd](../../aspose.note/documentvisitor/visitinkdrawingend/)(InkDrawing) | End to visit the [`InkDrawing`](../inkdrawing/) node. |
| virtual [VisitInkDrawingStart](../../aspose.note/documentvisitor/visitinkdrawingstart/)(InkDrawing) | Start to visit the [`InkDrawing`](../inkdrawing/) node. |
| virtual [VisitInkParagraphEnd](../../aspose.note/documentvisitor/visitinkparagraphend/)(InkParagraph) | End to visit the [`InkParagraph`](../inkparagraph/) node. |
| virtual [VisitInkParagraphStart](../../aspose.note/documentvisitor/visitinkparagraphstart/)(InkParagraph) | Start to visit the [`InkParagraph`](../inkparagraph/) node. |
| virtual [VisitInkWordEnd](../../aspose.note/documentvisitor/visitinkwordend/)(InkWord) | End to visit the [`InkWord`](../inkword/) node. |
| virtual [VisitInkWordStart](../../aspose.note/documentvisitor/visitinkwordstart/)(InkWord) | Start to visit the [`InkWord`](../inkword/) node. |
| virtual [VisitOutlineElementEnd](../../aspose.note/documentvisitor/visitoutlineelementend/)(OutlineElement) | End to visit the [`OutlineElement`](../outlineelement/) node. |
| virtual [VisitOutlineElementStart](../../aspose.note/documentvisitor/visitoutlineelementstart/)(OutlineElement) | Start to visit the [`OutlineElement`](../outlineelement/) node. |
| virtual [VisitOutlineEnd](../../aspose.note/documentvisitor/visitoutlineend/)(Outline) | End to visit the [`Outline`](../outline/) node. |
| virtual [VisitOutlineGroupEnd](../../aspose.note/documentvisitor/visitoutlinegroupend/)(OutlineGroup) | End to visit the [`OutlineGroup`](../outlinegroup/) node. |
| virtual [VisitOutlineGroupStart](../../aspose.note/documentvisitor/visitoutlinegroupstart/)(OutlineGroup) | Start to visit the [`OutlineGroup`](../outlinegroup/) node. |
| virtual [VisitOutlineStart](../../aspose.note/documentvisitor/visitoutlinestart/)(Outline) | Start to visit the [`Outline`](../outline/) node. |
| virtual [VisitPageEnd](../../aspose.note/documentvisitor/visitpageend/)(Page) | End to visit the [`Page`](../page/) node. |
| virtual [VisitPageStart](../../aspose.note/documentvisitor/visitpagestart/)(Page) | Start to visit the [`Page`](../page/) node. |
| virtual [VisitRichTextEnd](../../aspose.note/documentvisitor/visitrichtextend/)(RichText) | End to visit the [`RichText`](../richtext/) node. |
| virtual [VisitRichTextStart](../../aspose.note/documentvisitor/visitrichtextstart/)(RichText) | Start to visit the [`RichText`](../richtext/) node. |
| virtual [VisitTableCellEnd](../../aspose.note/documentvisitor/visittablecellend/)(TableCell) | End to visit the [`TableCell`](../tablecell/) node. |
| virtual [VisitTableCellStart](../../aspose.note/documentvisitor/visittablecellstart/)(TableCell) | Start to visit the [`TableCell`](../tablecell/) node. |
| virtual [VisitTableEnd](../../aspose.note/documentvisitor/visittableend/)(Table) | End to visit the [`Table`](../table/) node. |
| virtual [VisitTableRowEnd](../../aspose.note/documentvisitor/visittablerowend/)(TableRow) | End to visit the [`TableRow`](../tablerow/) node. |
| virtual [VisitTableRowStart](../../aspose.note/documentvisitor/visittablerowstart/)(TableRow) | Start to visit the [`TableRow`](../tablerow/) node. |
| virtual [VisitTableStart](../../aspose.note/documentvisitor/visittablestart/)(Table) | Start to visit the [`Table`](../table/) node. |
| virtual [VisitTitleEnd](../../aspose.note/documentvisitor/visittitleend/)(Title) | End to visit the [`Title`](../title/) node. |
| virtual [VisitTitleStart](../../aspose.note/documentvisitor/visittitlestart/)(Title) | Start to visit the [`Title`](../title/) node. |

## Examples

Shows how to access content of a document using visitor.

```csharp
public static void Run()
{
    // The path to the documents directory.
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // Open the document we want to convert.
    Document doc = new Document(dataDir + "Aspose.one");

    // Create an object that inherits from the DocumentVisitor class.
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // This is the well known Visitor pattern. Get the model to accept a visitor.
    // The model will iterate through itself by calling the corresponding methods
    // on the visitor object (this is called visiting).
    //
    // Note that every node in the object model has the Accept method so the visiting
    // can be executed not only for the whole document, but for any node in the document.
    doc.Accept(myConverter);

    // Once the visiting is complete, we can retrieve the result of the operation,
    // that in this example, has accumulated in the visitor.
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// Simple implementation of saving a document in the plain text format. Implemented as a Visitor.
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
    /// Gets the plain text of the document that was accumulated by the visitor.
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// Adds text to the current output. Honors the enabled/disabled output flag.
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// Called when a RichText node is encountered in the document.
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// Called when a Document node is encountered in the document.
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// Called when a Page node is encountered in the document.
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// Called when processing of a Page node is finished.
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// Called when a Title node is encountered in the document.
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// Called when a Image node is encountered in the document.
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// Called when a OutlineGroup node is encountered in the document.
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// Called when a Outline node is encountered in the document.
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// Called when a OutlineElement node is encountered in the document.
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// Gets the total count of nodes by the Visitor
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

### See Also

* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


