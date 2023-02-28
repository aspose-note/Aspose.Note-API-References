---
title: Page.GetChildNodes
second_title: Aspose.Note for .NET API Reference
description: Page μέθοδος. Λήψη όλων των θυγατρικών κόμβων της σελίδας ανά τύπο κόμβου.
type: docs
weight: 150
url: /el/net/aspose.note/page/getchildnodes/
---
## Page.GetChildNodes&lt;T1&gt; method

Λήψη όλων των θυγατρικών κόμβων της σελίδας ανά τύπο κόμβου.

```csharp
public override List<T1> GetChildNodes<T1>()
    where T1 : class, INode
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| T1 | Ο τύπος των στοιχείων στη λίστα που επιστρέφεται. |

### Επιστρεφόμενη Αξία

Μια λίστα με θυγατρικούς κόμβους.

### Παραδείγματα

Δείχνει πώς να λαμβάνετε όλο το κείμενο από το έγγραφο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Text();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Ανάκτηση κειμένου
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// Εκτύπωση κειμένου στην οθόνη εξόδου
Console.WriteLine(text);
```

Δείχνει πώς να λαμβάνετε όλο το κείμενο από τη σελίδα.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Text();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Λήψη λίστας κόμβων σελίδας
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // Ανάκτηση κειμένου
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // Εκτύπωση κειμένου στην οθόνη εξόδου
    Console.WriteLine(text);
}
```

Δείχνει πώς να περάσετε από όλες τις σελίδες και να κάνετε μια αντικατάσταση στο κείμενο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Λήψη όλων των κόμβων RichText
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Αντικατάσταση κειμένου σχήματος
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

// Αποθήκευση σε οποιαδήποτε υποστηριζόμενη μορφή αρχείου
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Δείχνει πώς να περάσετε μέσα από το κείμενο της σελίδας και να κάνετε μια αντικατάσταση.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// Λήψη όλων των κόμβων RichText
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Αντικατάσταση κειμένου σχήματος
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// Αποθήκευση σε οποιαδήποτε υποστηριζόμενη μορφή αρχείου
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

### Δείτε επίσης

* interface [INode](../../inode/)
* class [Page](../)
* χώρος ονομάτων [Aspose.Note](../../page/)
* συνέλευση [Aspose.Note](../../../)


