---
title: Document.Accept
second_title: Aspose.Note voor .NET API-referentie
description: Document methode. Accepteert de bezoeker van de node.
type: docs
weight: 80
url: /nl/net/aspose.note/document/accept/
---
## Document.Accept method

Accepteert de bezoeker van de node.

```csharp
public override void Accept(DocumentVisitor visitor)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| visitor | DocumentVisitor | Het object van een klasse afgeleid van de[`DocumentVisitor`](../../documentvisitor/) . |

### Voorbeelden

Laat zien hoe u toegang krijgt tot de inhoud van een document met behulp van bezoeker.

```csharp
public static void Run()
{
    // Het pad naar de documentenmap.
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // Open het document dat we willen converteren.
    Document doc = new Document(dataDir + "Aspose.one");

    // Maak een object dat overerft van de klasse DocumentVisitor.
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // Dit is het bekende Visitor-patroon. Laat het model een bezoeker accepteren.
    // Het model herhaalt zichzelf door de overeenkomstige methoden aan te roepen
    // op het bezoekersobject (dit wordt bezoeken genoemd).
    //
    // Merk op dat elk knooppunt in het objectmodel de Accept-methode heeft, dus het bezoeken
    // kan niet alleen voor het hele document worden uitgevoerd, maar voor elk knooppunt in het document.
    doc.Accept(myConverter);

    // Zodra het bezoek is voltooid, kunnen we het resultaat van de operatie ophalen,
    // die zich in dit voorbeeld heeft opgehoopt in de bezoeker.
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// Eenvoudige implementatie van het opslaan van een document in platte tekst. Geïmplementeerd als bezoeker.
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
    /// Krijgt de platte tekst van het document dat door de bezoeker is verzameld.
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// Voegt tekst toe aan de huidige uitvoer. Eert de uitvoervlag ingeschakeld/uitgeschakeld.
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// Aangeroepen wanneer een RichText-knooppunt wordt aangetroffen in het document.
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// Aangeroepen wanneer een documentknooppunt wordt aangetroffen in het document.
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// Aangeroepen wanneer een paginaknooppunt wordt aangetroffen in het document.
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// Opgeroepen wanneer de verwerking van een paginaknooppunt is voltooid.
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// Aangeroepen wanneer een titelknooppunt wordt aangetroffen in het document.
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// Aangeroepen wanneer een afbeeldingsknooppunt wordt aangetroffen in het document.
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// Aangeroepen wanneer een OutlineGroup-knooppunt wordt aangetroffen in het document.
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// Aangeroepen wanneer een Outline-knooppunt wordt aangetroffen in het document.
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// Aangeroepen wanneer een OutlineElement-knooppunt wordt aangetroffen in het document.
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// Krijgt het totale aantal nodes van de bezoeker
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

### Zie ook

* class [DocumentVisitor](../../documentvisitor/)
* class [Document](../)
* naamruimte [Aspose.Note](../../document/)
* montage [Aspose.Note](../../../)


