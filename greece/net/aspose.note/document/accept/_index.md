---
title: Document.Accept
second_title: Aspose.Note for .NET API Reference
description: Document μέθοδος. Αποδέχεται τον επισκέπτη του κόμβου.
type: docs
weight: 80
url: /el/net/aspose.note/document/accept/
---
## Document.Accept method

Αποδέχεται τον επισκέπτη του κόμβου.

```csharp
public override void Accept(DocumentVisitor visitor)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| visitor | DocumentVisitor | Το αντικείμενο μιας κλάσης που προέρχεται από το[`DocumentVisitor`](../../documentvisitor/) . |

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

* class [DocumentVisitor](../../documentvisitor/)
* class [Document](../)
* χώρος ονομάτων [Aspose.Note](../../document/)
* συνέλευση [Aspose.Note](../../../)


