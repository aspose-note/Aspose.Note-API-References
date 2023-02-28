---
title: Page.GetChildNodes
second_title: Aspose.Note för .NET API-referens
description: Page metod. Hämta alla underordnade noder på sidan efter nodtyp.
type: docs
weight: 150
url: /sv/net/aspose.note/page/getchildnodes/
---
## Page.GetChildNodes&lt;T1&gt; method

Hämta alla underordnade noder på sidan efter nodtyp.

```csharp
public override List<T1> GetChildNodes<T1>()
    where T1 : class, INode
```

| Parameter | Beskrivning |
| --- | --- |
| T1 | Typen av element i den returnerade listan. |

### Returvärde

En lista över underordnade noder.

### Exempel

Visar hur man hämtar all text från dokumentet.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Text();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Hämta text
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// Skriv ut text på utdataskärmen
Console.WriteLine(text);
```

Visar hur man hämtar all text från sidan.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Text();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Få lista över sidnoder
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // Hämta text
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // Skriv ut text på utdataskärmen
    Console.WriteLine(text);
}
```

Visar hur man går igenom alla sidor och gör en ersättning i texten.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Hämta alla RichText-noder
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Ersätt text i en form
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

// Spara till valfritt filformat som stöds
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Visar hur man går igenom sidans text och gör en ersättning.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// Hämta alla RichText-noder
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Ersätt text i en form
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// Spara till valfritt filformat som stöds
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

### Se även

* interface [INode](../../inode/)
* class [Page](../)
* namnutrymme [Aspose.Note](../../page/)
* hopsättning [Aspose.Note](../../../)


