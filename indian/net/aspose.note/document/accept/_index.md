---
title: Document.Accept
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Document तरक. नड के आगंतुक क स्वकर करत है
type: docs
weight: 80
url: /hi/net/aspose.note/document/accept/
---
## Document.Accept method

नोड के आगंतुक को स्वीकार करता है।

```csharp
public override void Accept(DocumentVisitor visitor)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| visitor | DocumentVisitor | से प्राप्त वर्ग की वस्तु[`DocumentVisitor`](../../documentvisitor/) . |

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

* class [DocumentVisitor](../../documentvisitor/)
* class [Document](../)
* नाम स्थान [Aspose.Note](../../document/)
* सभा [Aspose.Note](../../../)


