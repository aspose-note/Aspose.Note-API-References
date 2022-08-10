---
title: DocumentVisitor
second_title: Aspose.Note per .NET API Reference
description: La classe astratta per literazione del sottoalbero con root nel nodo specificato.
type: docs
weight: 70
url: /it/net/aspose.note/documentvisitor/
---
## DocumentVisitor class

La classe astratta per l'iterazione del sottoalbero con root nel nodo specificato.

```csharp
public abstract class DocumentVisitor
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| virtual [VisitAttachedFileEnd](../../aspose.note/documentvisitor/visitattachedfileend)(AttachedFile) | Fine per visitare il[`AttachedFile`](../attachedfile) nodo. |
| virtual [VisitAttachedFileStart](../../aspose.note/documentvisitor/visitattachedfilestart)(AttachedFile) | Inizia a visitare il[`AttachedFile`](../attachedfile) nodo. |
| virtual [VisitDocumentEnd](../../aspose.note/documentvisitor/visitdocumentend)(Document) | Fine per visitare il[`Document`](../document) nodo. |
| virtual [VisitDocumentStart](../../aspose.note/documentvisitor/visitdocumentstart)(Document) | Inizia a visitare il[`Document`](../document) nodo. |
| virtual [VisitImageEnd](../../aspose.note/documentvisitor/visitimageend)(Image) | Fine per visitare il[`Image`](../image) nodo. |
| virtual [VisitImageStart](../../aspose.note/documentvisitor/visitimagestart)(Image) | Inizia a visitare il[`Image`](../image) nodo. |
| virtual [VisitOutlineElementEnd](../../aspose.note/documentvisitor/visitoutlineelementend)(OutlineElement) | Fine per visitare il[`OutlineElement`](../outlineelement) nodo. |
| virtual [VisitOutlineElementStart](../../aspose.note/documentvisitor/visitoutlineelementstart)(OutlineElement) | Inizia a visitare il[`OutlineElement`](../outlineelement) nodo. |
| virtual [VisitOutlineEnd](../../aspose.note/documentvisitor/visitoutlineend)(Outline) | Fine per visitare il[`Outline`](../outline) nodo. |
| virtual [VisitOutlineGroupEnd](../../aspose.note/documentvisitor/visitoutlinegroupend)(OutlineGroup) | Fine per visitare il[`OutlineGroup`](../outlinegroup) nodo. |
| virtual [VisitOutlineGroupStart](../../aspose.note/documentvisitor/visitoutlinegroupstart)(OutlineGroup) | Inizia a visitare il[`OutlineGroup`](../outlinegroup) nodo. |
| virtual [VisitOutlineStart](../../aspose.note/documentvisitor/visitoutlinestart)(Outline) | Inizia a visitare il[`Outline`](../outline) nodo. |
| virtual [VisitPageEnd](../../aspose.note/documentvisitor/visitpageend)(Page) | Fine per visitare il[`Page`](../page) nodo. |
| virtual [VisitPageStart](../../aspose.note/documentvisitor/visitpagestart)(Page) | Inizia a visitare il[`Page`](../page) nodo. |
| virtual [VisitRichTextEnd](../../aspose.note/documentvisitor/visitrichtextend)(RichText) | Fine per visitare il[`RichText`](../richtext) nodo. |
| virtual [VisitRichTextStart](../../aspose.note/documentvisitor/visitrichtextstart)(RichText) | Inizia a visitare il[`RichText`](../richtext) nodo. |
| virtual [VisitTableCellEnd](../../aspose.note/documentvisitor/visittablecellend)(TableCell) | Fine per visitare il[`TableCell`](../tablecell) nodo. |
| virtual [VisitTableCellStart](../../aspose.note/documentvisitor/visittablecellstart)(TableCell) | Inizia a visitare il[`TableCell`](../tablecell) nodo. |
| virtual [VisitTableEnd](../../aspose.note/documentvisitor/visittableend)(Table) | Fine per visitare il[`Table`](../table) nodo. |
| virtual [VisitTableRowEnd](../../aspose.note/documentvisitor/visittablerowend)(TableRow) | Fine per visitare il[`TableRow`](../tablerow) nodo. |
| virtual [VisitTableRowStart](../../aspose.note/documentvisitor/visittablerowstart)(TableRow) | Inizia a visitare il[`TableRow`](../tablerow) nodo. |
| virtual [VisitTableStart](../../aspose.note/documentvisitor/visittablestart)(Table) | Inizia a visitare il[`Table`](../table) nodo. |
| virtual [VisitTitleEnd](../../aspose.note/documentvisitor/visittitleend)(Title) | Fine per visitare il[`Title`](../title) nodo. |
| virtual [VisitTitleStart](../../aspose.note/documentvisitor/visittitlestart)(Title) | Inizia a visitare il[`Title`](../title) nodo. |

### Esempi

Mostra come accedere al contenuto di un documento utilizzando il visitatore.

```csharp
public static void Run()
{
    // Il percorso della directory dei documenti.
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // Apri il documento che vogliamo convertire.
    Document doc = new Document(dataDir + "Aspose.one");

    // Crea un oggetto che eredita dalla classe DocumentVisitor.
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // Questo è il noto modello Visitor. Ottieni il modello per accettare un visitatore.
    // Il modello eseguirà un'iterazione su se stesso chiamando i metodi corrispondenti
    // sull'oggetto visitatore (questo è chiamato visita).
    //
    // Nota che ogni nodo nel modello a oggetti ha il metodo Accept, quindi la visita
    // può essere eseguito non solo per l'intero documento, ma per qualsiasi nodo nel documento.
    doc.Accept(myConverter);

    // Una volta completata la visita, possiamo recuperare il risultato dell'operazione,
    // che in questo esempio si è accumulato nel visitatore.
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// Semplice implementazione del salvataggio di un documento in formato testo normale. Implementato come visitatore.
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
    /// Ottiene il testo normale del documento accumulato dal visitatore.
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// Aggiunge testo all'output corrente. Rispetta il flag di uscita abilitato/disabilitato.
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// Chiamato quando viene rilevato un nodo RichText nel documento.
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// Chiamato quando viene rilevato un nodo Document nel documento.
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// Chiamato quando viene rilevato un nodo Pagina nel documento.
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// Chiamato quando l'elaborazione di un nodo Pagina è terminata.
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// Chiamato quando viene rilevato un nodo Titolo nel documento.
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// Chiamato quando viene rilevato un nodo Immagine nel documento.
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// Chiamato quando viene rilevato un nodo OutlineGroup nel documento.
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// Chiamato quando viene rilevato un nodo Struttura nel documento.
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// Chiamato quando viene rilevato un nodo OutlineElement nel documento.
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// Ottiene il conteggio totale dei nodi dal Visitatore
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

### Guarda anche

* spazio dei nomi [Aspose.Note](../../aspose.note)
* assemblea [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
