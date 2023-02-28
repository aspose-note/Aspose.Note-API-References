---
title: Class DocumentVisitor
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.DocumentVisitor कक्ष. नर्दष्ट नड पर रूट के सथ सबट्र के मध्यम से पुनरवृत के लए सर वर्ग
type: docs
weight: 70
url: /hi/net/aspose.note/documentvisitor/
---
## DocumentVisitor class

निर्दिष्ट नोड पर रूट के साथ सबट्री के माध्यम से पुनरावृति के लिए सार वर्ग।

```csharp
public abstract class DocumentVisitor
```

## तरीकों

| नाम | विवरण |
| --- | --- |
| virtual [VisitAttachedFileEnd](../../aspose.note/documentvisitor/visitattachedfileend/)(AttachedFile) | पर जाना समाप्त करें[`AttachedFile`](../attachedfile/) नोड. |
| virtual [VisitAttachedFileStart](../../aspose.note/documentvisitor/visitattachedfilestart/)(AttachedFile) | पर जाना शुरू करें[`AttachedFile`](../attachedfile/) नोड. |
| virtual [VisitDocumentEnd](../../aspose.note/documentvisitor/visitdocumentend/)(Document) | पर जाना समाप्त करें[`Document`](../document/) नोड. |
| virtual [VisitDocumentStart](../../aspose.note/documentvisitor/visitdocumentstart/)(Document) | पर जाना शुरू करें[`Document`](../document/) नोड. |
| virtual [VisitImageEnd](../../aspose.note/documentvisitor/visitimageend/)(Image) | पर जाना समाप्त करें[`Image`](../image/) नोड. |
| virtual [VisitImageStart](../../aspose.note/documentvisitor/visitimagestart/)(Image) | पर जाना शुरू करें[`Image`](../image/) नोड. |
| virtual [VisitOutlineElementEnd](../../aspose.note/documentvisitor/visitoutlineelementend/)(OutlineElement) | पर जाना समाप्त करें[`OutlineElement`](../outlineelement/) नोड. |
| virtual [VisitOutlineElementStart](../../aspose.note/documentvisitor/visitoutlineelementstart/)(OutlineElement) | पर जाना शुरू करें[`OutlineElement`](../outlineelement/) नोड. |
| virtual [VisitOutlineEnd](../../aspose.note/documentvisitor/visitoutlineend/)(Outline) | पर जाना समाप्त करें[`Outline`](../outline/) नोड. |
| virtual [VisitOutlineGroupEnd](../../aspose.note/documentvisitor/visitoutlinegroupend/)(OutlineGroup) | पर जाना समाप्त करें[`OutlineGroup`](../outlinegroup/) नोड. |
| virtual [VisitOutlineGroupStart](../../aspose.note/documentvisitor/visitoutlinegroupstart/)(OutlineGroup) | पर जाना शुरू करें[`OutlineGroup`](../outlinegroup/) नोड. |
| virtual [VisitOutlineStart](../../aspose.note/documentvisitor/visitoutlinestart/)(Outline) | पर जाना शुरू करें[`Outline`](../outline/) नोड. |
| virtual [VisitPageEnd](../../aspose.note/documentvisitor/visitpageend/)(Page) | पर जाना समाप्त करें[`Page`](../page/) नोड. |
| virtual [VisitPageStart](../../aspose.note/documentvisitor/visitpagestart/)(Page) | पर जाना शुरू करें[`Page`](../page/) नोड. |
| virtual [VisitRichTextEnd](../../aspose.note/documentvisitor/visitrichtextend/)(RichText) | पर जाना समाप्त करें[`RichText`](../richtext/) नोड. |
| virtual [VisitRichTextStart](../../aspose.note/documentvisitor/visitrichtextstart/)(RichText) | पर जाना शुरू करें[`RichText`](../richtext/) नोड. |
| virtual [VisitTableCellEnd](../../aspose.note/documentvisitor/visittablecellend/)(TableCell) | पर जाना समाप्त करें[`TableCell`](../tablecell/) नोड. |
| virtual [VisitTableCellStart](../../aspose.note/documentvisitor/visittablecellstart/)(TableCell) | पर जाना शुरू करें[`TableCell`](../tablecell/) नोड. |
| virtual [VisitTableEnd](../../aspose.note/documentvisitor/visittableend/)(Table) | पर जाना समाप्त करें[`Table`](../table/) नोड. |
| virtual [VisitTableRowEnd](../../aspose.note/documentvisitor/visittablerowend/)(TableRow) | पर जाना समाप्त करें[`TableRow`](../tablerow/) नोड. |
| virtual [VisitTableRowStart](../../aspose.note/documentvisitor/visittablerowstart/)(TableRow) | पर जाना शुरू करें[`TableRow`](../tablerow/) नोड. |
| virtual [VisitTableStart](../../aspose.note/documentvisitor/visittablestart/)(Table) | पर जाना शुरू करें[`Table`](../table/) नोड. |
| virtual [VisitTitleEnd](../../aspose.note/documentvisitor/visittitleend/)(Title) | पर जाना समाप्त करें[`Title`](../title/) नोड. |
| virtual [VisitTitleStart](../../aspose.note/documentvisitor/visittitlestart/)(Title) | पर जाना शुरू करें[`Title`](../title/) नोड. |

### उदाहरण

विज़िटर का उपयोग करके किसी दस्तावेज़ की सामग्री तक पहुँचने का तरीका दिखाता है।

```csharp
public static void Run()
{
    // दस्तावेज़ निर्देशिका का पथ।
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // वह दस्तावेज़ खोलें जिसे हम कनवर्ट करना चाहते हैं।
    Document doc = new Document(dataDir + "Aspose.one");

    // एक ऐसी वस्तु बनाएँ जो DocumentVisitor वर्ग से विरासत में मिली हो।
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // यह प्रसिद्ध विज़िटर पैटर्न है। एक आगंतुक को स्वीकार करने के लिए मॉडल प्राप्त करें।
    // संबंधित विधियों को कॉल करके मॉडल स्वयं के माध्यम से पुनरावृति करेगा
    // विज़िटर ऑब्जेक्ट पर (इसे विज़िटिंग कहा जाता है)।
    //
    // ध्यान दें कि ऑब्जेक्ट मॉडल में प्रत्येक नोड में एक्सेप्ट मेथड है इसलिए विजिटिंग
    // न केवल पूरे दस्तावेज़ के लिए, बल्कि दस्तावेज़ में किसी भी नोड के लिए निष्पादित किया जा सकता है।
    doc.Accept(myConverter);

    // एक बार दौरा पूरा हो जाने के बाद, हम ऑपरेशन के परिणाम को पुनः प्राप्त कर सकते हैं,
    // कि इस उदाहरण में, विज़िटर में जमा हो गया है।
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// सादे पाठ प्रारूप में दस्तावेज़ को सहेजने का सरल कार्यान्वयन। एक आगंतुक के रूप में लागू किया गया।
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
    /// आगंतुक द्वारा जमा किए गए दस्तावेज़ का सादा पाठ प्राप्त करता है।
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// वर्तमान आउटपुट में टेक्स्ट जोड़ता है। सक्षम/अक्षम आउटपुट फ़्लैग का सम्मान करता है।
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// जब दस्तावेज़ में एक RichText नोड का सामना किया जाता है तो कॉल किया जाता है।
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// जब दस्तावेज़ में दस्तावेज़ नोड का सामना किया जाता है तो कॉल किया जाता है।
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// कॉल किया जाता है जब दस्तावेज़ में पृष्ठ नोड का सामना होता है।
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// पेज नोड की प्रोसेसिंग समाप्त होने पर कॉल किया जाता है।
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// जब दस्तावेज़ में शीर्षक नोड का सामना किया जाता है तो कॉल किया जाता है।
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// दस्तावेज़ में एक छवि नोड का सामना करने पर कॉल किया जाता है।
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// कॉल किया जाता है जब दस्तावेज़ में एक OutlineGroup नोड का सामना होता है।
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// कॉल किया जाता है जब दस्तावेज़ में एक रूपरेखा नोड का सामना करना पड़ता है।
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// कॉल किया जाता है जब दस्तावेज़ में एक OutlineElement नोड का सामना होता है।
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// विज़िटर द्वारा नोड्स की कुल संख्या प्राप्त करता है
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

### यह सभी देखें

* नाम स्थान [Aspose.Note](../../aspose.note/)
* सभा [Aspose.Note](../../)


