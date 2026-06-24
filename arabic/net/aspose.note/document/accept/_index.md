---
title: "Document.Accept"
second_title: "مرجع API لـ Aspose.Note لـ .NET"
description: "طريقة Document. تقبل الزائر للعقدة"
type: docs
weight: 80
url: /ar/net/aspose.note/document/accept/
---
## Document.Accept method

يقبل زائر العقدة.

```csharp
public override void Accept(DocumentVisitor visitor)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| visitor | DocumentVisitor | الكائن من فئة مشتقة من [`DocumentVisitor`](../../documentvisitor/). |

## أمثلة

يظهر كيفية الوصول إلى محتوى مستند باستخدام الزائر.

```csharp
public static void Run()
{
    // المسار إلى دليل المستندات.
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // افتح المستند الذي نريد تحويله.
    Document doc = new Document(dataDir + "Aspose.one");

    // أنشئ كائنًا يرث من الفئة **DocumentVisitor**.
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // هذا هو نمط Visitor المعروف جيدًا. اجعل النموذج يقبل زائرًا.
    // سيقوم النموذج بالتكرار على نفسه عن طريق استدعاء الطرق المقابلة
    // على كائن الزائر (هذا ما يُسمى بالزيارة).
    //
    // لاحظ أن كل عقدة في نموذج الكائن لديها طريقة Accept لذا يمكن تنفيذ الزيارة
    // ليس فقط للمستند الكامل، بل لأي عقدة في المستند.
    doc.Accept(myConverter);

    // بمجرد اكتمال الزيارة، يمكننا استرجاع نتيجة العملية،
    // التي في هذا المثال، تم تجميعها في الزائر.
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// تنفيذ بسيط لحفظ مستند بتنسيق النص العادي. تم تنفيذها كـ Visitor.
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
    /// يحصل على النص العادي للمستند الذي تم تجميعه بواسطة الزائر.
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// يضيف نصًا إلى الإخراج الحالي. يراعي علم الإخراج المفعّل/المعطّل.
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// يُستدعى عندما يتم العثور على عقدة RichText في المستند.
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// يُستدعى عندما يتم العثور على عقدة Document في المستند.
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// يُستدعى عندما يتم العثور على عقدة Page في المستند.
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// يُستدعى عندما ينتهي معالجة عقدة Page.
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// يُستدعى عندما يتم العثور على عقدة Title في المستند.
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// يُستدعى عندما يتم العثور على عقدة Image في المستند.
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// يُستدعى عندما يتم العثور على عقدة OutlineGroup في المستند.
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// يُستدعى عندما يتم العثور على عقدة Outline في المستند.
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// يُستدعى عندما يتم العثور على عقدة OutlineElement في المستند.
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// يحصل على العدد الكلي للعقد بواسطة Visitor
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

### انظر أيضًا

* class [DocumentVisitor](../../documentvisitor/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)


