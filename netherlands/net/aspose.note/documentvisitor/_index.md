---
title: Class DocumentVisitor
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.DocumentVisitor klas. De abstracte klasse voor iteratie door substructuur met root op het gespecificeerde knooppunt.
type: docs
weight: 70
url: /nl/net/aspose.note/documentvisitor/
---
## DocumentVisitor class

De abstracte klasse voor iteratie door substructuur met root op het gespecificeerde knooppunt.

```csharp
public abstract class DocumentVisitor
```

## methoden

| Naam | Beschrijving |
| --- | --- |
| virtual [VisitAttachedFileEnd](../../aspose.note/documentvisitor/visitattachedfileend/)(AttachedFile) | Einde om de te bezoeken[`AttachedFile`](../attachedfile/) knooppunt. |
| virtual [VisitAttachedFileStart](../../aspose.note/documentvisitor/visitattachedfilestart/)(AttachedFile) | Begin met het bezoeken van de[`AttachedFile`](../attachedfile/) knooppunt. |
| virtual [VisitDocumentEnd](../../aspose.note/documentvisitor/visitdocumentend/)(Document) | Einde om de te bezoeken[`Document`](../document/) knooppunt. |
| virtual [VisitDocumentStart](../../aspose.note/documentvisitor/visitdocumentstart/)(Document) | Begin met het bezoeken van de[`Document`](../document/) knooppunt. |
| virtual [VisitImageEnd](../../aspose.note/documentvisitor/visitimageend/)(Image) | Einde om de te bezoeken[`Image`](../image/) knooppunt. |
| virtual [VisitImageStart](../../aspose.note/documentvisitor/visitimagestart/)(Image) | Begin met het bezoeken van de[`Image`](../image/) knooppunt. |
| virtual [VisitOutlineElementEnd](../../aspose.note/documentvisitor/visitoutlineelementend/)(OutlineElement) | Einde om de te bezoeken[`OutlineElement`](../outlineelement/) knooppunt. |
| virtual [VisitOutlineElementStart](../../aspose.note/documentvisitor/visitoutlineelementstart/)(OutlineElement) | Begin met het bezoeken van de[`OutlineElement`](../outlineelement/) knooppunt. |
| virtual [VisitOutlineEnd](../../aspose.note/documentvisitor/visitoutlineend/)(Outline) | Einde om de te bezoeken[`Outline`](../outline/) knooppunt. |
| virtual [VisitOutlineGroupEnd](../../aspose.note/documentvisitor/visitoutlinegroupend/)(OutlineGroup) | Einde om de te bezoeken[`OutlineGroup`](../outlinegroup/) knooppunt. |
| virtual [VisitOutlineGroupStart](../../aspose.note/documentvisitor/visitoutlinegroupstart/)(OutlineGroup) | Begin met het bezoeken van de[`OutlineGroup`](../outlinegroup/) knooppunt. |
| virtual [VisitOutlineStart](../../aspose.note/documentvisitor/visitoutlinestart/)(Outline) | Begin met het bezoeken van de[`Outline`](../outline/) knooppunt. |
| virtual [VisitPageEnd](../../aspose.note/documentvisitor/visitpageend/)(Page) | Einde om de te bezoeken[`Page`](../page/) knooppunt. |
| virtual [VisitPageStart](../../aspose.note/documentvisitor/visitpagestart/)(Page) | Begin met het bezoeken van de[`Page`](../page/) knooppunt. |
| virtual [VisitRichTextEnd](../../aspose.note/documentvisitor/visitrichtextend/)(RichText) | Einde om de te bezoeken[`RichText`](../richtext/) knooppunt. |
| virtual [VisitRichTextStart](../../aspose.note/documentvisitor/visitrichtextstart/)(RichText) | Begin met het bezoeken van de[`RichText`](../richtext/) knooppunt. |
| virtual [VisitTableCellEnd](../../aspose.note/documentvisitor/visittablecellend/)(TableCell) | Einde om de te bezoeken[`TableCell`](../tablecell/) knooppunt. |
| virtual [VisitTableCellStart](../../aspose.note/documentvisitor/visittablecellstart/)(TableCell) | Begin met het bezoeken van de[`TableCell`](../tablecell/) knooppunt. |
| virtual [VisitTableEnd](../../aspose.note/documentvisitor/visittableend/)(Table) | Einde om de te bezoeken[`Table`](../table/) knooppunt. |
| virtual [VisitTableRowEnd](../../aspose.note/documentvisitor/visittablerowend/)(TableRow) | Einde om de te bezoeken[`TableRow`](../tablerow/) knooppunt. |
| virtual [VisitTableRowStart](../../aspose.note/documentvisitor/visittablerowstart/)(TableRow) | Begin met het bezoeken van de[`TableRow`](../tablerow/) knooppunt. |
| virtual [VisitTableStart](../../aspose.note/documentvisitor/visittablestart/)(Table) | Begin met het bezoeken van de[`Table`](../table/) knooppunt. |
| virtual [VisitTitleEnd](../../aspose.note/documentvisitor/visittitleend/)(Title) | Einde om de te bezoeken[`Title`](../title/) knooppunt. |
| virtual [VisitTitleStart](../../aspose.note/documentvisitor/visittitlestart/)(Title) | Begin met het bezoeken van de[`Title`](../title/) knooppunt. |

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

* naamruimte [Aspose.Note](../../aspose.note/)
* montage [Aspose.Note](../../)


