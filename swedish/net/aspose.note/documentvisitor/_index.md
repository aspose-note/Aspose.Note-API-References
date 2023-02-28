---
title: Class DocumentVisitor
second_title: Aspose.Note för .NET API-referens
description: Aspose.Note.DocumentVisitor klass. Den abstrakta klassen för iterering genom underträd med rot vid den angivna noden.
type: docs
weight: 70
url: /sv/net/aspose.note/documentvisitor/
---
## DocumentVisitor class

Den abstrakta klassen för iterering genom underträd med rot vid den angivna noden.

```csharp
public abstract class DocumentVisitor
```

## Metoder

| namn | Beskrivning |
| --- | --- |
| virtual [VisitAttachedFileEnd](../../aspose.note/documentvisitor/visitattachedfileend/)(AttachedFile) | Avsluta för att besöka[`AttachedFile`](../attachedfile/) nod. |
| virtual [VisitAttachedFileStart](../../aspose.note/documentvisitor/visitattachedfilestart/)(AttachedFile) | Börja besöka[`AttachedFile`](../attachedfile/) nod. |
| virtual [VisitDocumentEnd](../../aspose.note/documentvisitor/visitdocumentend/)(Document) | Avsluta för att besöka[`Document`](../document/) nod. |
| virtual [VisitDocumentStart](../../aspose.note/documentvisitor/visitdocumentstart/)(Document) | Börja besöka[`Document`](../document/) nod. |
| virtual [VisitImageEnd](../../aspose.note/documentvisitor/visitimageend/)(Image) | Avsluta för att besöka[`Image`](../image/) nod. |
| virtual [VisitImageStart](../../aspose.note/documentvisitor/visitimagestart/)(Image) | Börja besöka[`Image`](../image/) nod. |
| virtual [VisitOutlineElementEnd](../../aspose.note/documentvisitor/visitoutlineelementend/)(OutlineElement) | Avsluta för att besöka[`OutlineElement`](../outlineelement/) nod. |
| virtual [VisitOutlineElementStart](../../aspose.note/documentvisitor/visitoutlineelementstart/)(OutlineElement) | Börja besöka[`OutlineElement`](../outlineelement/) nod. |
| virtual [VisitOutlineEnd](../../aspose.note/documentvisitor/visitoutlineend/)(Outline) | Avsluta för att besöka[`Outline`](../outline/) nod. |
| virtual [VisitOutlineGroupEnd](../../aspose.note/documentvisitor/visitoutlinegroupend/)(OutlineGroup) | Avsluta för att besöka[`OutlineGroup`](../outlinegroup/) nod. |
| virtual [VisitOutlineGroupStart](../../aspose.note/documentvisitor/visitoutlinegroupstart/)(OutlineGroup) | Börja besöka[`OutlineGroup`](../outlinegroup/) nod. |
| virtual [VisitOutlineStart](../../aspose.note/documentvisitor/visitoutlinestart/)(Outline) | Börja besöka[`Outline`](../outline/) nod. |
| virtual [VisitPageEnd](../../aspose.note/documentvisitor/visitpageend/)(Page) | Avsluta för att besöka[`Page`](../page/) nod. |
| virtual [VisitPageStart](../../aspose.note/documentvisitor/visitpagestart/)(Page) | Börja besöka[`Page`](../page/) nod. |
| virtual [VisitRichTextEnd](../../aspose.note/documentvisitor/visitrichtextend/)(RichText) | Avsluta för att besöka[`RichText`](../richtext/) nod. |
| virtual [VisitRichTextStart](../../aspose.note/documentvisitor/visitrichtextstart/)(RichText) | Börja besöka[`RichText`](../richtext/) nod. |
| virtual [VisitTableCellEnd](../../aspose.note/documentvisitor/visittablecellend/)(TableCell) | Avsluta för att besöka[`TableCell`](../tablecell/) nod. |
| virtual [VisitTableCellStart](../../aspose.note/documentvisitor/visittablecellstart/)(TableCell) | Börja besöka[`TableCell`](../tablecell/) nod. |
| virtual [VisitTableEnd](../../aspose.note/documentvisitor/visittableend/)(Table) | Avsluta för att besöka[`Table`](../table/) nod. |
| virtual [VisitTableRowEnd](../../aspose.note/documentvisitor/visittablerowend/)(TableRow) | Avsluta för att besöka[`TableRow`](../tablerow/) nod. |
| virtual [VisitTableRowStart](../../aspose.note/documentvisitor/visittablerowstart/)(TableRow) | Börja besöka[`TableRow`](../tablerow/) nod. |
| virtual [VisitTableStart](../../aspose.note/documentvisitor/visittablestart/)(Table) | Börja besöka[`Table`](../table/) nod. |
| virtual [VisitTitleEnd](../../aspose.note/documentvisitor/visittitleend/)(Title) | Avsluta för att besöka[`Title`](../title/) nod. |
| virtual [VisitTitleStart](../../aspose.note/documentvisitor/visittitlestart/)(Title) | Börja besöka[`Title`](../title/) nod. |

### Exempel

Visar hur man kommer åt innehållet i ett dokument med hjälp av besökare.

```csharp
public static void Run()
{
    // Sökvägen till dokumentkatalogen.
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // Öppna dokumentet vi vill konvertera.
    Document doc = new Document(dataDir + "Aspose.one");

    // Skapa ett objekt som ärver från klassen DocumentVisitor.
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // Detta är det välkända besökarmönstret. Få modellen att ta emot en besökare.
    // Modellen kommer att iterera genom sig själv genom att anropa motsvarande metoder
    // på besöksobjektet (detta kallas att besöka).
    //
    // Observera att varje nod i objektmodellen har Accept-metoden så att den besöker
    // kan köras inte bara för hela dokumentet, utan för vilken nod som helst i dokumentet.
    doc.Accept(myConverter);

    // När besöket är klart kan vi hämta resultatet av operationen,
    // som i det här exemplet har ackumulerats i besökaren.
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// Enkel implementering av att spara ett dokument i vanlig textformat. Implementerad som besökare.
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
    /// Hämtar vanlig text av dokumentet som samlades av besökaren.
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// Lägger till text till den aktuella utgången. Respekterar den aktiverade/avaktiverade utgångsflaggan.
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// Anropas när en RichText-nod påträffas i dokumentet.
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// Anropas när en dokumentnod påträffas i dokumentet.
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// Anropas när en sidnod påträffas i dokumentet.
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// Anropas när bearbetningen av en sidnod är klar.
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// Anropas när en titelnod påträffas i dokumentet.
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// Anropas när en bildnod påträffas i dokumentet.
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// Anropas när en OutlineGroup-nod påträffas i dokumentet.
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// Anropas när en Outline-nod påträffas i dokumentet.
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// Anropas när en OutlineElement-nod påträffas i dokumentet.
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// Får det totala antalet noder av besökaren
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

### Se även

* namnutrymme [Aspose.Note](../../aspose.note/)
* hopsättning [Aspose.Note](../../)


