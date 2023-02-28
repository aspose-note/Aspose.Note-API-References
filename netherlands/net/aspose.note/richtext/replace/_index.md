---
title: RichText.Replace
second_title: Aspose.Note voor .NET API-referentie
description: RichText methode. Vervangt alle exemplaren van een opgegeven Unicodeteken in deze instantie door een ander opgegeven Unicodeteken.
type: docs
weight: 200
url: /nl/net/aspose.note/richtext/replace/
---
## Replace(char, char) {#replace}

Vervangt alle exemplaren van een opgegeven Unicode-teken in deze instantie door een ander opgegeven Unicode-teken.

```csharp
public RichText Replace(char oldChar, char newChar)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| oldChar | Char | De oude char. |
| newChar | Char | De nieuwe char. |

### Winstwaarde

De[`RichText`](../) .

### Zie ook

* class [RichText](../)
* naamruimte [Aspose.Note](../../richtext/)
* montage [Aspose.Note](../../../)

---

## Replace(string, string) {#replace_1}

Vervangt alle exemplaren van een opgegeven tekenreeks in de huidige instantie door een andere opgegeven tekenreeks.

```csharp
public RichText Replace(string oldValue, string newValue)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| oldValue | String | De oude waarde. |
| newValue | String | De nieuwe waarde. |

### Winstwaarde

De[`RichText`](../) .

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

### Voorbeelden

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

Laat zien hoe u een nieuw document kunt genereren door speciale tekststukken in een sjabloon te vervangen.

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

// Laad het sjabloondocument in Aspose.Note.
var d = new Document(Path.Combine(dataDir, "JobOffer.one"));

// Laten we alle sjabloonwoorden vervangen
foreach (var e in d.GetChildNodes<RichText>())
{
    foreach (var replace in D)
    {
        e.Replace($"${{{replace.Key}}}", replace.Value);
    }
}

d.Save(Path.Combine(dataDir, "JobOffer_out.one"));
```

### Zie ook

* class [RichText](../)
* naamruimte [Aspose.Note](../../richtext/)
* montage [Aspose.Note](../../../)

---

## Replace(string, string, TextStyle) {#replace_2}

Vervangt alle exemplaren van een opgegeven tekenreeks in de huidige instantie door een andere opgegeven tekenreeks in opgegeven stijl.

```csharp
public RichText Replace(string oldValue, string newValue, TextStyle style)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| oldValue | String | De oude waarde. |
| newValue | String | De nieuwe waarde. |
| style | TextStyle | De stijl van de nieuwe waarde. |

### Winstwaarde

De[`RichText`](../) .

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

### Zie ook

* class [TextStyle](../../textstyle/)
* class [RichText](../)
* naamruimte [Aspose.Note](../../richtext/)
* montage [Aspose.Note](../../../)


