---
title: DocumentFontsSubsystem.UsingDefaultFont
second_title: Aspose.Note för .NET API-referens
description: DocumentFontsSubsystem metod. Skapa ny DocumentFontsSubsysteminstans med det angivna standardteckensnittsnamnet.
type: docs
weight: 30
url: /sv/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfont/
---
## DocumentFontsSubsystem.UsingDefaultFont method

Skapa ny DocumentFontsSubsystem-instans med det angivna standardteckensnittsnamnet.

```csharp
public static DocumentFontsSubsystem UsingDefaultFont(string defaultFontName, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| defaultFontName | String | Standardteckensnittsnamnet. |
| fontsSubstitutions | Dictionary`2 | Teckensnittsersättningarna. |

### Returvärde

Den[`DocumentFontsSubsystem`](../) .

### Exempel

Visar hur man sparar ett dokument i pdf-format med angivet standardteckensnitt.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Spara dokumentet som PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

### Se även

* class [DocumentFontsSubsystem](../)
* namnutrymme [Aspose.Note.Fonts](../../documentfontssubsystem/)
* hopsättning [Aspose.Note](../../../)


