---
title: Class DocumentVisitor
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.DocumentVisitor τάξη. Η αφηρημένη κλάση για επανάληψη μέσω υποδέντρου με ρίζα στον καθορισμένο κόμβο.
type: docs
weight: 70
url: /el/net/aspose.note/documentvisitor/
---
## DocumentVisitor class

Η αφηρημένη κλάση για επανάληψη μέσω υποδέντρου με ρίζα στον καθορισμένο κόμβο.

```csharp
public abstract class DocumentVisitor
```

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| virtual [VisitAttachedFileEnd](../../aspose.note/documentvisitor/visitattachedfileend/)(AttachedFile) | Τέλος για να επισκεφθείτε το[`AttachedFile`](../attachedfile/) κόμβος. |
| virtual [VisitAttachedFileStart](../../aspose.note/documentvisitor/visitattachedfilestart/)(AttachedFile) | Ξεκινήστε να επισκέπτεστε το[`AttachedFile`](../attachedfile/) κόμβος. |
| virtual [VisitDocumentEnd](../../aspose.note/documentvisitor/visitdocumentend/)(Document) | Τέλος για να επισκεφθείτε το[`Document`](../document/) κόμβος. |
| virtual [VisitDocumentStart](../../aspose.note/documentvisitor/visitdocumentstart/)(Document) | Ξεκινήστε να επισκέπτεστε το[`Document`](../document/) κόμβος. |
| virtual [VisitImageEnd](../../aspose.note/documentvisitor/visitimageend/)(Image) | Τέλος για να επισκεφθείτε το[`Image`](../image/) κόμβος. |
| virtual [VisitImageStart](../../aspose.note/documentvisitor/visitimagestart/)(Image) | Ξεκινήστε να επισκέπτεστε το[`Image`](../image/) κόμβος. |
| virtual [VisitOutlineElementEnd](../../aspose.note/documentvisitor/visitoutlineelementend/)(OutlineElement) | Τέλος για να επισκεφθείτε το[`OutlineElement`](../outlineelement/) κόμβος. |
| virtual [VisitOutlineElementStart](../../aspose.note/documentvisitor/visitoutlineelementstart/)(OutlineElement) | Ξεκινήστε να επισκέπτεστε το[`OutlineElement`](../outlineelement/) κόμβος. |
| virtual [VisitOutlineEnd](../../aspose.note/documentvisitor/visitoutlineend/)(Outline) | Τέλος για να επισκεφθείτε το[`Outline`](../outline/) κόμβος. |
| virtual [VisitOutlineGroupEnd](../../aspose.note/documentvisitor/visitoutlinegroupend/)(OutlineGroup) | Τέλος για να επισκεφθείτε το[`OutlineGroup`](../outlinegroup/) κόμβος. |
| virtual [VisitOutlineGroupStart](../../aspose.note/documentvisitor/visitoutlinegroupstart/)(OutlineGroup) | Ξεκινήστε να επισκέπτεστε το[`OutlineGroup`](../outlinegroup/) κόμβος. |
| virtual [VisitOutlineStart](../../aspose.note/documentvisitor/visitoutlinestart/)(Outline) | Ξεκινήστε να επισκέπτεστε το[`Outline`](../outline/) κόμβος. |
| virtual [VisitPageEnd](../../aspose.note/documentvisitor/visitpageend/)(Page) | Τέλος για να επισκεφθείτε το[`Page`](../page/) κόμβος. |
| virtual [VisitPageStart](../../aspose.note/documentvisitor/visitpagestart/)(Page) | Ξεκινήστε να επισκέπτεστε το[`Page`](../page/) κόμβος. |
| virtual [VisitRichTextEnd](../../aspose.note/documentvisitor/visitrichtextend/)(RichText) | Τέλος για να επισκεφθείτε το[`RichText`](../richtext/) κόμβος. |
| virtual [VisitRichTextStart](../../aspose.note/documentvisitor/visitrichtextstart/)(RichText) | Ξεκινήστε να επισκέπτεστε το[`RichText`](../richtext/) κόμβος. |
| virtual [VisitTableCellEnd](../../aspose.note/documentvisitor/visittablecellend/)(TableCell) | Τέλος για να επισκεφθείτε το[`TableCell`](../tablecell/) κόμβος. |
| virtual [VisitTableCellStart](../../aspose.note/documentvisitor/visittablecellstart/)(TableCell) | Ξεκινήστε να επισκέπτεστε το[`TableCell`](../tablecell/) κόμβος. |
| virtual [VisitTableEnd](../../aspose.note/documentvisitor/visittableend/)(Table) | Τέλος για να επισκεφθείτε το[`Table`](../table/) κόμβος. |
| virtual [VisitTableRowEnd](../../aspose.note/documentvisitor/visittablerowend/)(TableRow) | Τέλος για να επισκεφθείτε το[`TableRow`](../tablerow/) κόμβος. |
| virtual [VisitTableRowStart](../../aspose.note/documentvisitor/visittablerowstart/)(TableRow) | Ξεκινήστε να επισκέπτεστε το[`TableRow`](../tablerow/) κόμβος. |
| virtual [VisitTableStart](../../aspose.note/documentvisitor/visittablestart/)(Table) | Ξεκινήστε να επισκέπτεστε το[`Table`](../table/) κόμβος. |
| virtual [VisitTitleEnd](../../aspose.note/documentvisitor/visittitleend/)(Title) | Τέλος για να επισκεφθείτε το[`Title`](../title/) κόμβος. |
| virtual [VisitTitleStart](../../aspose.note/documentvisitor/visittitlestart/)(Title) | Ξεκινήστε να επισκέπτεστε το[`Title`](../title/) κόμβος. |

### Παραδείγματα

Δείχνει τον τρόπο πρόσβασης στο περιεχόμενο ενός εγγράφου χρησιμοποιώντας τον επισκέπτη.

```csharp
public static void Run()
{
    // Η διαδρομή προς τον κατάλογο εγγράφων.
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // Ανοίξτε το έγγραφο που θέλουμε να μετατρέψουμε.
    Document doc = new Document(dataDir + "Aspose.one");

    // Δημιουργήστε ένα αντικείμενο που κληρονομεί από την κλάση DocumentVisitor.
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // Αυτό είναι το γνωστό μοτίβο επισκεπτών. Πάρτε το μοντέλο για να δεχτεί έναν επισκέπτη.
    // Το μοντέλο θα επαναληφθεί μέσω του εαυτού του καλώντας τις αντίστοιχες μεθόδους
    // στο αντικείμενο επισκέπτη (αυτό ονομάζεται επίσκεψη).
    //
    // Σημειώστε ότι κάθε κόμβος στο μοντέλο αντικειμένου έχει τη μέθοδο Accept και έτσι την επίσκεψη
    // μπορεί να εκτελεστεί όχι μόνο για ολόκληρο το έγγραφο, αλλά για οποιονδήποτε κόμβο του εγγράφου.
    doc.Accept(myConverter);

    // Μόλις ολοκληρωθεί η επίσκεψη, μπορούμε να ανακτήσουμε το αποτέλεσμα της λειτουργίας,
    // που σε αυτό το παράδειγμα, έχει συσσωρευτεί στον επισκέπτη.
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// Απλή υλοποίηση της αποθήκευσης ενός εγγράφου σε μορφή απλού κειμένου. Υλοποιήθηκε ως Επισκέπτης.
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
    /// Λαμβάνει το απλό κείμενο του εγγράφου που συγκεντρώθηκε από τον επισκέπτη.
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// Προσθέτει κείμενο στην τρέχουσα έξοδο. Τιμά τη σημαία ενεργοποίησης/απενεργοποίησης εξόδου.
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// Καλείται όταν εμφανίζεται ένας κόμβος εμπλουτισμένου κειμένου στο έγγραφο.
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// Καλείται όταν συναντάται ένας κόμβος εγγράφου στο έγγραφο.
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// Καλείται όταν εμφανίζεται ένας κόμβος σελίδας στο έγγραφο.
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// Καλείται όταν ολοκληρωθεί η επεξεργασία ενός κόμβου Σελίδας.
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// Καλείται όταν βρεθεί ένας κόμβος τίτλου στο έγγραφο.
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// Καλείται όταν εμφανίζεται ένας κόμβος εικόνας στο έγγραφο.
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// Καλείται όταν ένας κόμβος OutlineGroup συναντάται στο έγγραφο.
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// Καλείται όταν συναντάται ένας κόμβος Outline στο έγγραφο.
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// Καλείται όταν εμφανίζεται ένας κόμβος OutlineElement στο έγγραφο.
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// Λαμβάνει τον συνολικό αριθμό των κόμβων από τον Επισκέπτη
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

### Δείτε επίσης

* χώρος ονομάτων [Aspose.Note](../../aspose.note/)
* συνέλευση [Aspose.Note](../../)


