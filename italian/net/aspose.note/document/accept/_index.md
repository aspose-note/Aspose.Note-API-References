---
title: Document.Accept
second_title: Aspose.Note per .NET API Reference
description: Document metodo. Accetta il visitatore del nodo.
type: docs
weight: 80
url: /it/net/aspose.note/document/accept/
---
## Document.Accept method

Accetta il visitatore del nodo.

```csharp
public override void Accept(DocumentVisitor visitor)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| visitor | DocumentVisitor | L'oggetto di una classe derivata da[`DocumentVisitor`](../../documentvisitor/) . |

### Esempi

Mostra come accedere al contenuto di un documento utilizzando il visitatore.

```csharp
public static void Run()
{
    // Il percorso della directory dei documenti.
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // Apre il documento che vogliamo convertire.
    Document doc = new Document(dataDir + "Aspose.one");

    // Crea un oggetto che eredita dalla classe DocumentVisitor.
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // Questo è il noto pattern Visitor. Fai in modo che il modello accetti un visitatore.
    // Il modello ripeterà se stesso chiamando i metodi corrispondenti
    // sull'oggetto visitatore (questo si chiama visiting).
    //
    // Si noti che ogni nodo nel modello a oggetti ha il metodo Accept, quindi visiting
    // può essere eseguito non solo per l'intero documento, ma per qualsiasi nodo nel documento.
    doc.Accept(myConverter);

    // Una volta completata la visita, possiamo recuperare il risultato dell'operazione,
    // che in questo esempio si è accumulato nel visitatore.
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// Semplice implementazione del salvataggio di un documento nel formato testo normale. Implementato come visitatore.
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
    /// Aggiunge testo all'output corrente. Rispetta il flag di output abilitato/disabilitato.
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// Chiamato quando si incontra un nodo RichText nel documento.
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// Chiamato quando si incontra un nodo Documento nel documento.
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// Chiamato quando si incontra un nodo Page nel documento.
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// Chiamato quando l'elaborazione di un nodo Page è terminata.
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// Chiamato quando si incontra un nodo Title nel documento.
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// Chiamato quando si incontra un nodo Image nel documento.
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// Chiamato quando si incontra un nodo OutlineGroup nel documento.
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// Chiamato quando si incontra un nodo Struttura nel documento.
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
    /// Ottiene il conteggio totale dei nodi del visitatore
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

* class [DocumentVisitor](../../documentvisitor/)
* class [Document](../)
* spazio dei nomi [Aspose.Note](../../document/)
* assemblea [Aspose.Note](../../../)


