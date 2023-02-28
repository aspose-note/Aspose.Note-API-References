---
title: DocumentFontsSubsystem.UsingDefaultFontFromStream
second_title: Aspose.Note voor .NET API-referentie
description: DocumentFontsSubsystem methode. Maak een nieuwe DocumentFontsSubsysteminstantie met standaard een lettertype uit de opgegeven stream.
type: docs
weight: 50
url: /nl/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream/
---
## DocumentFontsSubsystem.UsingDefaultFontFromStream method

Maak een nieuwe DocumentFontsSubsystem-instantie met standaard een lettertype uit de opgegeven stream.

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromStream(Stream defaultFontStream, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| defaultFontStream | Stream | De stream met de standaardlettertypenaam. |
| fontsSubstitutions | Dictionary`2 | De vervangingen van lettertypen. |

### Winstwaarde

De[`DocumentFontsSubsystem`](../) .

### Voorbeelden

Laat zien hoe u een document in pdf-indeling opslaat met het standaardlettertype van een stream.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Laad het document in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Sla het document op als PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### Zie ook

* class [DocumentFontsSubsystem](../)
* naamruimte [Aspose.Note.Fonts](../../documentfontssubsystem/)
* montage [Aspose.Note](../../../)


