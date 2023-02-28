---
title: RichText.Replace
second_title: Aspose.Note für .NET-API-Referenz
description: RichText methode. Ersetzt alle Vorkommen eines angegebenen UnicodeZeichens in dieser Instanz durch ein anderes angegebenes UnicodeZeichen.
type: docs
weight: 200
url: /de/net/aspose.note/richtext/replace/
---
## Replace(char, char) {#replace}

Ersetzt alle Vorkommen eines angegebenen Unicode-Zeichens in dieser Instanz durch ein anderes angegebenes Unicode-Zeichen.

```csharp
public RichText Replace(char oldChar, char newChar)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| oldChar | Char | Das alte Zeichen. |
| newChar | Char | Das neue Zeichen. |

### Rückgabewert

Die[`RichText`](../) .

### Siehe auch

* class [RichText](../)
* namensraum [Aspose.Note](../../richtext/)
* Montage [Aspose.Note](../../../)

---

## Replace(string, string) {#replace_1}

Ersetzt alle Vorkommen einer angegebenen Zeichenfolge in der aktuellen Instanz durch eine andere angegebene Zeichenfolge.

```csharp
public RichText Replace(string oldValue, string newValue)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| oldValue | String | Der alte Wert. |
| newValue | String | Der neue Wert. |

### Rückgabewert

Die[`RichText`](../) .

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

### Beispiele

Zeigt, wie man den Text der Seite durchläuft und eine Ersetzung vornimmt.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// Alle RichText-Knoten abrufen
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Text einer Form ersetzen
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// In jedem unterstützten Dateiformat speichern
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Zeigt, wie ein neues Dokument generiert wird, indem spezielle Textteile in einer Vorlage ersetzt werden.

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

// Laden Sie das Vorlagendokument in Aspose.Note.
var d = new Document(Path.Combine(dataDir, "JobOffer.one"));

// Lassen Sie uns alle Vorlagenwörter ersetzen
foreach (var e in d.GetChildNodes<RichText>())
{
    foreach (var replace in D)
    {
        e.Replace($"${{{replace.Key}}}", replace.Value);
    }
}

d.Save(Path.Combine(dataDir, "JobOffer_out.one"));
```

### Siehe auch

* class [RichText](../)
* namensraum [Aspose.Note](../../richtext/)
* Montage [Aspose.Note](../../../)

---

## Replace(string, string, TextStyle) {#replace_2}

Ersetzt alle Vorkommen einer angegebenen Zeichenfolge in der aktuellen Instanz durch eine andere angegebene Zeichenfolge im angegebenen Stil.

```csharp
public RichText Replace(string oldValue, string newValue, TextStyle style)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| oldValue | String | Der alte Wert. |
| newValue | String | Der neue Wert. |
| style | TextStyle | Der Stil des neuen Werts. |

### Rückgabewert

Die[`RichText`](../) .

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

### Siehe auch

* class [TextStyle](../../textstyle/)
* class [RichText](../)
* namensraum [Aspose.Note](../../richtext/)
* Montage [Aspose.Note](../../../)


