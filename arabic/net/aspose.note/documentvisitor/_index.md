---
title: Class DocumentVisitor
second_title: Aspose.Note لمرجع NET API
description: Aspose.Note.DocumentVisitor فصل. فئة مجردة للتكرار خلال الشجرة الفرعية مع الجذر في العقدة المحددة.
type: docs
weight: 70
url: /ar/net/aspose.note/documentvisitor/
---
## DocumentVisitor class

فئة مجردة للتكرار خلال الشجرة الفرعية مع الجذر في العقدة المحددة.

```csharp
public abstract class DocumentVisitor
```

## طُرق

| اسم | وصف |
| --- | --- |
| virtual [VisitAttachedFileEnd](../../aspose.note/documentvisitor/visitattachedfileend/)(AttachedFile) | نهاية لزيارة[`AttachedFile`](../attachedfile/) العقدة . |
| virtual [VisitAttachedFileStart](../../aspose.note/documentvisitor/visitattachedfilestart/)(AttachedFile) | ابدأ بزيارة موقع[`AttachedFile`](../attachedfile/) العقدة . |
| virtual [VisitDocumentEnd](../../aspose.note/documentvisitor/visitdocumentend/)(Document) | نهاية لزيارة[`Document`](../document/) العقدة . |
| virtual [VisitDocumentStart](../../aspose.note/documentvisitor/visitdocumentstart/)(Document) | ابدأ بزيارة موقع[`Document`](../document/) العقدة . |
| virtual [VisitImageEnd](../../aspose.note/documentvisitor/visitimageend/)(Image) | نهاية لزيارة[`Image`](../image/) العقدة . |
| virtual [VisitImageStart](../../aspose.note/documentvisitor/visitimagestart/)(Image) | ابدأ بزيارة موقع[`Image`](../image/) العقدة . |
| virtual [VisitOutlineElementEnd](../../aspose.note/documentvisitor/visitoutlineelementend/)(OutlineElement) | نهاية لزيارة[`OutlineElement`](../outlineelement/) العقدة . |
| virtual [VisitOutlineElementStart](../../aspose.note/documentvisitor/visitoutlineelementstart/)(OutlineElement) | ابدأ بزيارة موقع[`OutlineElement`](../outlineelement/) العقدة . |
| virtual [VisitOutlineEnd](../../aspose.note/documentvisitor/visitoutlineend/)(Outline) | نهاية لزيارة[`Outline`](../outline/) العقدة . |
| virtual [VisitOutlineGroupEnd](../../aspose.note/documentvisitor/visitoutlinegroupend/)(OutlineGroup) | نهاية لزيارة[`OutlineGroup`](../outlinegroup/) العقدة . |
| virtual [VisitOutlineGroupStart](../../aspose.note/documentvisitor/visitoutlinegroupstart/)(OutlineGroup) | ابدأ بزيارة موقع[`OutlineGroup`](../outlinegroup/) العقدة . |
| virtual [VisitOutlineStart](../../aspose.note/documentvisitor/visitoutlinestart/)(Outline) | ابدأ بزيارة موقع[`Outline`](../outline/) العقدة . |
| virtual [VisitPageEnd](../../aspose.note/documentvisitor/visitpageend/)(Page) | نهاية لزيارة[`Page`](../page/) العقدة . |
| virtual [VisitPageStart](../../aspose.note/documentvisitor/visitpagestart/)(Page) | ابدأ بزيارة موقع[`Page`](../page/) العقدة . |
| virtual [VisitRichTextEnd](../../aspose.note/documentvisitor/visitrichtextend/)(RichText) | نهاية لزيارة[`RichText`](../richtext/) العقدة . |
| virtual [VisitRichTextStart](../../aspose.note/documentvisitor/visitrichtextstart/)(RichText) | ابدأ بزيارة موقع[`RichText`](../richtext/) العقدة . |
| virtual [VisitTableCellEnd](../../aspose.note/documentvisitor/visittablecellend/)(TableCell) | نهاية لزيارة[`TableCell`](../tablecell/) العقدة . |
| virtual [VisitTableCellStart](../../aspose.note/documentvisitor/visittablecellstart/)(TableCell) | ابدأ بزيارة موقع[`TableCell`](../tablecell/) العقدة . |
| virtual [VisitTableEnd](../../aspose.note/documentvisitor/visittableend/)(Table) | نهاية لزيارة[`Table`](../table/) العقدة . |
| virtual [VisitTableRowEnd](../../aspose.note/documentvisitor/visittablerowend/)(TableRow) | نهاية لزيارة[`TableRow`](../tablerow/) العقدة . |
| virtual [VisitTableRowStart](../../aspose.note/documentvisitor/visittablerowstart/)(TableRow) | ابدأ بزيارة موقع[`TableRow`](../tablerow/) العقدة . |
| virtual [VisitTableStart](../../aspose.note/documentvisitor/visittablestart/)(Table) | ابدأ بزيارة موقع[`Table`](../table/) العقدة . |
| virtual [VisitTitleEnd](../../aspose.note/documentvisitor/visittitleend/)(Title) | نهاية لزيارة[`Title`](../title/) العقدة . |
| virtual [VisitTitleStart](../../aspose.note/documentvisitor/visittitlestart/)(Title) | ابدأ بزيارة موقع[`Title`](../title/) العقدة . |

### أمثلة

يوضح كيفية الوصول إلى محتوى مستند باستخدام الزائر.

```csharp
public static void Run()
{
    // المسار إلى دليل المستندات.
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // افتح المستند الذي نريد تحويله.
    Document doc = new Document(dataDir + "Aspose.one");

    // إنشاء كائن يرث من فئة DocumentVisitor.
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // هذا هو نمط الزائر المعروف. احصل على النموذج لقبول زائر.
    // سيقوم النموذج بالتكرار من خلال نفسه عن طريق استدعاء الطرق المقابلة
    // على كائن الزائر (وهذا ما يسمى بالزيارة).
    //
    // لاحظ أن كل عقدة في نموذج الكائن لها طريقة Accept لذا فإن زيارة
    يمكن تنفيذ // ليس فقط للمستند بأكمله ، ولكن لأي عقدة في المستند.
    doc.Accept(myConverter);

    // بمجرد اكتمال الزيارة ، يمكننا استرداد نتيجة العملية ،
    // التي في هذا المثال تراكمت في الزائر.
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// تنفيذ بسيط لحفظ مستند بتنسيق النص العادي. تم تنفيذه كزائر.
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
    /// يحصل على النص العادي للمستند الذي قام الزائر بتجميعه.
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// يضيف نصًا إلى الإخراج الحالي. يكرم علامة الإخراج الممكنة / المعطلة.
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// يتم الاستدعاء عند مواجهة عقدة RichText في المستند.
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// يتم الاستدعاء عند مواجهة عقدة المستند في المستند.
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// يتم استدعاؤها عند مواجهة عقدة الصفحة في المستند.
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// يتم الاستدعاء عند انتهاء معالجة عقدة الصفحة.
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// يتم استدعاؤها عند مواجهة عقدة العنوان في المستند.
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// يتم الاستدعاء عند مواجهة عقدة صورة في المستند.
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// يتم الاستدعاء عند مواجهة عقدة OutlineGroup في المستند.
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// يتم استدعاؤها عند مواجهة عقدة مخطط تفصيلي في المستند.
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// يتم استدعاؤه عند مواجهة عقدة OutlineElement في المستند.
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// الحصول على العدد الإجمالي للعقد بواسطة الزائر
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

### أنظر أيضا

* مساحة الاسم [Aspose.Note](../../aspose.note/)
* المجسم [Aspose.Note](../../)


