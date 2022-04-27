---
title: DocumentVisitor
second_title: Aspose.Note for .NET API Reference
description: 
type: docs
weight: 70
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
| virtual [VisitAttachedFileEnd](visitattachedfileend)(AttachedFile) | End to visit the [`AttachedFile`](../attachedfile) node. |
| virtual [VisitAttachedFileStart](visitattachedfilestart)(AttachedFile) | Start to visit the [`AttachedFile`](../attachedfile) node. |
| virtual [VisitDocumentEnd](visitdocumentend)(Document) | End to visit the [`Document`](../document) node. |
| virtual [VisitDocumentStart](visitdocumentstart)(Document) | Start to visit the [`Document`](../document) node. |
| virtual [VisitImageEnd](visitimageend)(Image) | End to visit the [`Image`](../image) node. |
| virtual [VisitImageStart](visitimagestart)(Image) | Start to visit the [`Image`](../image) node. |
| virtual [VisitOutlineElementEnd](visitoutlineelementend)(OutlineElement) | End to visit the [`OutlineElement`](../outlineelement) node. |
| virtual [VisitOutlineElementStart](visitoutlineelementstart)(OutlineElement) | Start to visit the [`OutlineElement`](../outlineelement) node. |
| virtual [VisitOutlineEnd](visitoutlineend)(Outline) | End to visit the [`Outline`](../outline) node. |
| virtual [VisitOutlineGroupEnd](visitoutlinegroupend)(OutlineGroup) | End to visit the [`OutlineGroup`](../outlinegroup) node. |
| virtual [VisitOutlineGroupStart](visitoutlinegroupstart)(OutlineGroup) | Start to visit the [`OutlineGroup`](../outlinegroup) node. |
| virtual [VisitOutlineStart](visitoutlinestart)(Outline) | Start to visit the [`Outline`](../outline) node. |
| virtual [VisitPageEnd](visitpageend)(Page) | End to visit the [`Page`](../page) node. |
| virtual [VisitPageStart](visitpagestart)(Page) | Start to visit the [`Page`](../page) node. |
| virtual [VisitRichTextEnd](visitrichtextend)(RichText) | End to visit the [`RichText`](../richtext) node. |
| virtual [VisitRichTextStart](visitrichtextstart)(RichText) | Start to visit the [`RichText`](../richtext) node. |
| virtual [VisitTableCellEnd](visittablecellend)(TableCell) | End to visit the [`TableCell`](../tablecell) node. |
| virtual [VisitTableCellStart](visittablecellstart)(TableCell) | Start to visit the [`TableCell`](../tablecell) node. |
| virtual [VisitTableEnd](visittableend)(Table) | End to visit the [`Table`](../table) node. |
| virtual [VisitTableRowEnd](visittablerowend)(TableRow) | End to visit the [`TableRow`](../tablerow) node. |
| virtual [VisitTableRowStart](visittablerowstart)(TableRow) | Start to visit the [`TableRow`](../tablerow) node. |
| virtual [VisitTableStart](visittablestart)(Table) | Start to visit the [`Table`](../table) node. |
| virtual [VisitTitleEnd](visittitleend)(Title) | End to visit the [`Title`](../title) node. |
| virtual [VisitTitleStart](visittitlestart)(Title) | Start to visit the [`Title`](../title) node. |

### Examples

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

* namespace [Aspose.Note](../../aspose.note)
* assembly [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
