---
title: RichText.Replace
second_title: Aspose.Note for .NET API Reference
description: RichText method. Replaces all occurrences of a specified Unicode character in this instance with another specified Unicode character
type: docs
weight: 200
url: /net/aspose.note/richtext/replace/
---
## Replace(char, char) {#replace}

Replaces all occurrences of a specified Unicode character in this instance with another specified Unicode character.

```csharp
public RichText Replace(char oldChar, char newChar)
```

| Parameter | Type | Description |
| --- | --- | --- |
| oldChar | Char | The old char. |
| newChar | Char | The new char. |

### Return Value

The [`RichText`](../).

### See Also

* class [RichText](../)
* namespace [Aspose.Note](../../richtext/)
* assembly [Aspose.Note](../../../)

---

## Replace(string, string) {#replace_1}

Replaces all occurrences of a specified string in the current instance with another specified string.

```csharp
public RichText Replace(string oldValue, string newValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| oldValue | String | The old value. |
| newValue | String | The new value. |

### Return Value

The [`RichText`](../).

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

## Examples

Shows how to pass through page's text and make a replacement.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// Get all RichText nodes
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Replace text of a shape
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// Save to any supported file format
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Shows how to generate a new document by replacing special text pieces in a template.

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

// Load the template document into Aspose.Note.
var d = new Document(Path.Combine(dataDir, "JobOffer.one"));

// Let's replace all template words
foreach (var e in d.GetChildNodes<RichText>())
{
    foreach (var replace in D)
    {
        e.Replace($"${{{replace.Key}}}", replace.Value);
    }
}

d.Save(Path.Combine(dataDir, "JobOffer_out.one"));
```

### See Also

* class [RichText](../)
* namespace [Aspose.Note](../../richtext/)
* assembly [Aspose.Note](../../../)

---

## Replace(string, string, TextStyle) {#replace_2}

Replaces all occurrences of a specified string in the current instance with another specified string in specified style.

```csharp
public RichText Replace(string oldValue, string newValue, TextStyle style)
```

| Parameter | Type | Description |
| --- | --- | --- |
| oldValue | String | The old value. |
| newValue | String | The new value. |
| style | TextStyle | The style of the new value. |

### Return Value

The [`RichText`](../).

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

### See Also

* class [TextStyle](../../textstyle/)
* class [RichText](../)
* namespace [Aspose.Note](../../richtext/)
* assembly [Aspose.Note](../../../)


