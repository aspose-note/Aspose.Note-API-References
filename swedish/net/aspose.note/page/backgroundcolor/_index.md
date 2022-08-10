---
title: BackgroundColor
second_title: Aspose.Note för .NET API-referens
description: Hämtar eller ställer in sidans bakgrundsfärg.
type: docs
weight: 30
url: /sv/net/aspose.note/page/backgroundcolor/
---
## Page.BackgroundColor property

Hämtar eller ställer in sidans bakgrundsfärg.

```csharp
public Color BackgroundColor { get; set; }
```

### Exempel

Visar hur du ställer in sidans bakgrundsfärg.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Pages();

// Ladda OneNote-dokument och skaffa första barn           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in document)
{
    page.BackgroundColor = Color.BlueViolet;
}

document.Save(Path.Combine(dataDir, "SetPageBackgroundColor.one"));
```

### Se även

* class [Page](../../page)
* namnutrymme [Aspose.Note](../../page)
* hopsättning [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->