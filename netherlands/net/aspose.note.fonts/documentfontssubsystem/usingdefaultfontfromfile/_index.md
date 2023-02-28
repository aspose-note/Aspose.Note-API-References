---
title: DocumentFontsSubsystem.UsingDefaultFontFromFile
second_title: Aspose.Note voor .NET API-referentie
description: DocumentFontsSubsystem methode. Maak een nieuwe DocumentFontsSubsysteminstantie met standaard een lettertype uit het opgegeven bestand.
type: docs
weight: 40
url: /nl/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/
---
## DocumentFontsSubsystem.UsingDefaultFontFromFile method

Maak een nieuwe DocumentFontsSubsystem-instantie met standaard een lettertype uit het opgegeven bestand.

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromFile(string filePath, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | String | Het bestand met de standaardlettertypenaam. |
| fontsSubstitutions | Dictionary`2 | De vervangingen van lettertypen. |

### Winstwaarde

De[`DocumentFontsSubsystem`](../) .

### Voorbeelden

Laat zien hoe u een document in pdf-indeling opslaat met het standaardlettertype uit een bestand.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Laad het document in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Sla het document op als PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

### Zie ook

* class [DocumentFontsSubsystem](../)
* naamruimte [Aspose.Note.Fonts](../../documentfontssubsystem/)
* montage [Aspose.Note](../../../)


