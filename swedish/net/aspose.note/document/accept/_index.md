---
title: Document.Accept
second_title: Aspose.Note för .NET API-referens
description: Document metod. Accepterar besökaren av noden.
type: docs
weight: 80
url: /sv/net/aspose.note/document/accept/
---
## Document.Accept method

Accepterar besökaren av noden.

```csharp
public override void Accept(DocumentVisitor visitor)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| visitor | DocumentVisitor | Objektet för en klass som härrör från[`DocumentVisitor`](../../documentvisitor/) . |

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

* class [DocumentVisitor](../../documentvisitor/)
* class [Document](../)
* namnutrymme [Aspose.Note](../../document/)
* hopsättning [Aspose.Note](../../../)


