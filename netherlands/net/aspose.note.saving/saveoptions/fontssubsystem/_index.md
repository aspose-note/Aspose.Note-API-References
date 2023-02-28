---
title: SaveOptions.FontsSubsystem
second_title: Aspose.Note voor .NET API-referentie
description: SaveOptions eigendom. Haalt lettertypeinstellingen op of stelt deze in om te gebruiken tijdens het opslaan
type: docs
weight: 10
url: /nl/net/aspose.note.saving/saveoptions/fontssubsystem/
---
## SaveOptions.FontsSubsystem property

Haalt lettertype-instellingen op of stelt deze in om te gebruiken tijdens het opslaan

```csharp
public FontsSubsystem FontsSubsystem { get; set; }
```

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

* class [FontsSubsystem](../../../aspose.note.fonts/fontssubsystem/)
* class [SaveOptions](../)
* naamruimte [Aspose.Note.Saving](../../saveoptions/)
* montage [Aspose.Note](../../../)


