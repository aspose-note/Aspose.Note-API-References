---
title: Class DocumentVisitor
second_title: Aspose.Note für .NET-API-Referenz
description: Aspose.Note.DocumentVisitor klas. Die abstrakte Klasse zum Iterieren durch den Teilbaum mit Wurzel am angegebenen Knoten.
type: docs
weight: 70
url: /de/net/aspose.note/documentvisitor/
---
## DocumentVisitor class

Die abstrakte Klasse zum Iterieren durch den Teilbaum mit Wurzel am angegebenen Knoten.

```csharp
public abstract class DocumentVisitor
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| virtual [VisitAttachedFileEnd](../../aspose.note/documentvisitor/visitattachedfileend/)(AttachedFile) | Ende zu besuchen[`AttachedFile`](../attachedfile/) Knoten. |
| virtual [VisitAttachedFileStart](../../aspose.note/documentvisitor/visitattachedfilestart/)(AttachedFile) | Beginnen Sie mit dem Besuch der[`AttachedFile`](../attachedfile/) Knoten. |
| virtual [VisitDocumentEnd](../../aspose.note/documentvisitor/visitdocumentend/)(Document) | Ende zu besuchen[`Document`](../document/) Knoten. |
| virtual [VisitDocumentStart](../../aspose.note/documentvisitor/visitdocumentstart/)(Document) | Beginnen Sie mit dem Besuch der[`Document`](../document/) Knoten. |
| virtual [VisitImageEnd](../../aspose.note/documentvisitor/visitimageend/)(Image) | Ende zu besuchen[`Image`](../image/) Knoten. |
| virtual [VisitImageStart](../../aspose.note/documentvisitor/visitimagestart/)(Image) | Beginnen Sie mit dem Besuch der[`Image`](../image/) Knoten. |
| virtual [VisitOutlineElementEnd](../../aspose.note/documentvisitor/visitoutlineelementend/)(OutlineElement) | Ende zu besuchen[`OutlineElement`](../outlineelement/) Knoten. |
| virtual [VisitOutlineElementStart](../../aspose.note/documentvisitor/visitoutlineelementstart/)(OutlineElement) | Beginnen Sie mit dem Besuch der[`OutlineElement`](../outlineelement/) Knoten. |
| virtual [VisitOutlineEnd](../../aspose.note/documentvisitor/visitoutlineend/)(Outline) | Ende zu besuchen[`Outline`](../outline/) Knoten. |
| virtual [VisitOutlineGroupEnd](../../aspose.note/documentvisitor/visitoutlinegroupend/)(OutlineGroup) | Ende zu besuchen[`OutlineGroup`](../outlinegroup/) Knoten. |
| virtual [VisitOutlineGroupStart](../../aspose.note/documentvisitor/visitoutlinegroupstart/)(OutlineGroup) | Beginnen Sie mit dem Besuch der[`OutlineGroup`](../outlinegroup/) Knoten. |
| virtual [VisitOutlineStart](../../aspose.note/documentvisitor/visitoutlinestart/)(Outline) | Beginnen Sie mit dem Besuch der[`Outline`](../outline/) Knoten. |
| virtual [VisitPageEnd](../../aspose.note/documentvisitor/visitpageend/)(Page) | Ende zu besuchen[`Page`](../page/) Knoten. |
| virtual [VisitPageStart](../../aspose.note/documentvisitor/visitpagestart/)(Page) | Beginnen Sie mit dem Besuch der[`Page`](../page/) Knoten. |
| virtual [VisitRichTextEnd](../../aspose.note/documentvisitor/visitrichtextend/)(RichText) | Ende zu besuchen[`RichText`](../richtext/) Knoten. |
| virtual [VisitRichTextStart](../../aspose.note/documentvisitor/visitrichtextstart/)(RichText) | Beginnen Sie mit dem Besuch der[`RichText`](../richtext/) Knoten. |
| virtual [VisitTableCellEnd](../../aspose.note/documentvisitor/visittablecellend/)(TableCell) | Ende zu besuchen[`TableCell`](../tablecell/) Knoten. |
| virtual [VisitTableCellStart](../../aspose.note/documentvisitor/visittablecellstart/)(TableCell) | Beginnen Sie mit dem Besuch der[`TableCell`](../tablecell/) Knoten. |
| virtual [VisitTableEnd](../../aspose.note/documentvisitor/visittableend/)(Table) | Ende zu besuchen[`Table`](../table/) Knoten. |
| virtual [VisitTableRowEnd](../../aspose.note/documentvisitor/visittablerowend/)(TableRow) | Ende zu besuchen[`TableRow`](../tablerow/) Knoten. |
| virtual [VisitTableRowStart](../../aspose.note/documentvisitor/visittablerowstart/)(TableRow) | Beginnen Sie mit dem Besuch der[`TableRow`](../tablerow/) Knoten. |
| virtual [VisitTableStart](../../aspose.note/documentvisitor/visittablestart/)(Table) | Beginnen Sie mit dem Besuch der[`Table`](../table/) Knoten. |
| virtual [VisitTitleEnd](../../aspose.note/documentvisitor/visittitleend/)(Title) | Ende zu besuchen[`Title`](../title/) Knoten. |
| virtual [VisitTitleStart](../../aspose.note/documentvisitor/visittitlestart/)(Title) | Beginnen Sie mit dem Besuch der[`Title`](../title/) Knoten. |

### Beispiele

Zeigt, wie Sie mit „Besucher“ auf den Inhalt eines Dokuments zugreifen.

```csharp
public static void Run()
{
    // Der Pfad zum Dokumentenverzeichnis.
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // Öffnen Sie das Dokument, das wir konvertieren möchten.
    Document doc = new Document(dataDir + "Aspose.one");

    // Ein Objekt erstellen, das von der DocumentVisitor-Klasse erbt.
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // Dies ist das bekannte Besuchermuster. Bringen Sie das Modell dazu, einen Besucher anzunehmen.
    // Das Modell iteriert durch sich selbst, indem es die entsprechenden Methoden aufruft
    // auf dem Besucherobjekt (dies wird Besuch genannt).
    //
    // Beachten Sie, dass jeder Knoten im Objektmodell die Accept-Methode hat, also den Besuch
    // kann nicht nur für das gesamte Dokument ausgeführt werden, sondern für jeden Knoten im Dokument.
    doc.Accept(myConverter);

    // Sobald der Besuch abgeschlossen ist, können wir das Ergebnis der Operation abrufen,
    // die sich in diesem Beispiel im Besucher angesammelt hat.
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// Einfache Implementierung zum Speichern eines Dokuments im Nur-Text-Format. Als Besucher implementiert.
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
    /// Ruft den Klartext des Dokuments ab, das vom Besucher angesammelt wurde.
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// Fügt Text zur aktuellen Ausgabe hinzu. Berücksichtigt das aktivierte/deaktivierte Ausgangsflag.
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// Wird aufgerufen, wenn im Dokument ein RichText-Knoten gefunden wird.
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// Wird aufgerufen, wenn im Dokument ein Dokumentknoten gefunden wird.
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// Wird aufgerufen, wenn im Dokument ein Page-Knoten gefunden wird.
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// Wird aufgerufen, wenn die Verarbeitung eines Seitenknotens abgeschlossen ist.
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// Wird aufgerufen, wenn im Dokument ein Titelknoten gefunden wird.
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// Wird aufgerufen, wenn im Dokument ein Image-Knoten gefunden wird.
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// Wird aufgerufen, wenn im Dokument ein OutlineGroup-Knoten gefunden wird.
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// Wird aufgerufen, wenn im Dokument ein Outline-Knoten gefunden wird.
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// Wird aufgerufen, wenn im Dokument ein OutlineElement-Knoten gefunden wird.
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// Ruft die Gesamtzahl der Knoten des Besuchers ab
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

### Siehe auch

* namensraum [Aspose.Note](../../aspose.note/)
* Montage [Aspose.Note](../../)


