---
title: Accept
second_title: Aspose.Note für .NET-API-Referenz
description: Akzeptiert den Besucher des Knotens.
type: docs
weight: 80
url: /de/net/aspose.note/document/accept/
---
## Document.Accept method

Akzeptiert den Besucher des Knotens.

```csharp
public override void Accept(DocumentVisitor visitor)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| visitor | DocumentVisitor | Das Objekt einer Klasse, abgeleitet von der[`DocumentVisitor`](../../documentvisitor) . |

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

* class [DocumentVisitor](../../documentvisitor)
* class [Document](../../document)
* namensraum [Aspose.Note](../../document)
* Montage [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
