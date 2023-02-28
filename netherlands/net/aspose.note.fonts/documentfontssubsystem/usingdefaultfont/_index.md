---
title: DocumentFontsSubsystem.UsingDefaultFont
second_title: Aspose.Note voor .NET API-referentie
description: DocumentFontsSubsystem methode. Maak een nieuwe DocumentFontsSubsysteminstantie met de opgegeven standaardlettertypenaam.
type: docs
weight: 30
url: /nl/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfont/
---
## DocumentFontsSubsystem.UsingDefaultFont method

Maak een nieuwe DocumentFontsSubsystem-instantie met de opgegeven standaardlettertypenaam.

```csharp
public static DocumentFontsSubsystem UsingDefaultFont(string defaultFontName, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| defaultFontName | String | De standaardlettertypenaam. |
| fontsSubstitutions | Dictionary`2 | De vervangingen van lettertypen. |

### Winstwaarde

De[`DocumentFontsSubsystem`](../) .

### Voorbeelden

Laat zien hoe u een document in pdf-indeling kunt opslaan met het opgegeven standaardlettertype.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Sla het document op als PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

### Zie ook

* class [DocumentFontsSubsystem](../)
* naamruimte [Aspose.Note.Fonts](../../documentfontssubsystem/)
* montage [Aspose.Note](../../../)


