---
title: Page.GetChildNodes
second_title: Aspose.Note voor .NET API-referentie
description: Page methode. Alle onderliggende knooppunten van de pagina ophalen op basis van het knooppunttype.
type: docs
weight: 150
url: /nl/net/aspose.note/page/getchildnodes/
---
## Page.GetChildNodes&lt;T1&gt; method

Alle onderliggende knooppunten van de pagina ophalen op basis van het knooppunttype.

```csharp
public override List<T1> GetChildNodes<T1>()
    where T1 : class, INode
```

| Parameter | Beschrijving |
| --- | --- |
| T1 | Het type elementen in de geretourneerde lijst. |

### Winstwaarde

Een lijst met onderliggende knooppunten.

### Voorbeelden

Laat zien hoe u alle tekst uit het document kunt halen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Text();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Tekst ophalen
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// Print tekst op het uitvoerscherm
Console.WriteLine(text);
```

Laat zien hoe u alle tekst van de pagina kunt halen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Text();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Krijg een lijst met paginaknooppunten
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // Tekst ophalen
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // Print tekst op het uitvoerscherm
    Console.WriteLine(text);
}
```

Laat zien hoe u alle pagina's kunt doorlopen en een vervanging in de tekst kunt maken.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Haal alle RichText-knooppunten op
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Vervang tekst van een vorm
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

// Sla op in elk ondersteund bestandsformaat
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Laat zien hoe u door de tekst van de pagina kunt gaan en een vervanging kunt maken.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// Haal alle RichText-knooppunten op
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Vervang tekst van een vorm
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// Sla op in elk ondersteund bestandsformaat
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

### Zie ook

* interface [INode](../../inode/)
* class [Page](../)
* naamruimte [Aspose.Note](../../page/)
* montage [Aspose.Note](../../../)


