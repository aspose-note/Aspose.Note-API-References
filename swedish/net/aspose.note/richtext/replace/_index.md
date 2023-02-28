---
title: RichText.Replace
second_title: Aspose.Note för .NET API-referens
description: RichText metod. Ersätter alla förekomster av ett specificerat Unicodetecken i det här fallet med ett annat specificerat Unicodetecken.
type: docs
weight: 200
url: /sv/net/aspose.note/richtext/replace/
---
## Replace(char, char) {#replace}

Ersätter alla förekomster av ett specificerat Unicode-tecken i det här fallet med ett annat specificerat Unicode-tecken.

```csharp
public RichText Replace(char oldChar, char newChar)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| oldChar | Char | Den gamla char. |
| newChar | Char | Den nya char. |

### Returvärde

Den[`RichText`](../) .

### Se även

* class [RichText](../)
* namnutrymme [Aspose.Note](../../richtext/)
* hopsättning [Aspose.Note](../../../)

---

## Replace(string, string) {#replace_1}

Ersätter alla förekomster av en angiven sträng i den aktuella instansen med en annan specificerad sträng.

```csharp
public RichText Replace(string oldValue, string newValue)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| oldValue | String | Det gamla värdet. |
| newValue | String | Det nya värdet. |

### Returvärde

Den[`RichText`](../) .

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

### Exempel

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

Visar hur man skapar ett nytt dokument genom att ersätta speciella textbitar i en mall.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

var D = new Dictionary<string, string>
            {
                { "Company", "Atlas Shrugged Ltd" },
                { "CandidateName", "John Galt" },
                { "JobTitle", "Chief Entrepreneur Officer" },
                { "Department", "Sales" },
                { "Salary", "123456 USD" },
                { "Vacation", "30" },
                { "StartDate", "29 Feb 2024" },
                { "YourName", "Ayn Rand" }
            };

// Ladda malldokumentet i Aspose.Note.
var d = new Document(Path.Combine(dataDir, "JobOffer.one"));

// Låt oss ersätta alla mallord
foreach (var e in d.GetChildNodes<RichText>())
{
    foreach (var replace in D)
    {
        e.Replace($"${{{replace.Key}}}", replace.Value);
    }
}

d.Save(Path.Combine(dataDir, "JobOffer_out.one"));
```

### Se även

* class [RichText](../)
* namnutrymme [Aspose.Note](../../richtext/)
* hopsättning [Aspose.Note](../../../)

---

## Replace(string, string, TextStyle) {#replace_2}

Ersätter alla förekomster av en angiven sträng i den aktuella instansen med en annan specificerad sträng i angiven stil.

```csharp
public RichText Replace(string oldValue, string newValue, TextStyle style)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| oldValue | String | Det gamla värdet. |
| newValue | String | Det nya värdet. |
| style | TextStyle | Stilen för det nya värdet. |

### Returvärde

Den[`RichText`](../) .

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

### Se även

* class [TextStyle](../../textstyle/)
* class [RichText](../)
* namnutrymme [Aspose.Note](../../richtext/)
* hopsättning [Aspose.Note](../../../)


