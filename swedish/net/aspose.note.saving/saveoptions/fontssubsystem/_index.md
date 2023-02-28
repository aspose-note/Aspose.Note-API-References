---
title: SaveOptions.FontsSubsystem
second_title: Aspose.Note för .NET API-referens
description: SaveOptions fast egendom. Hämtar eller ställer in teckensnittets inställningar som ska användas medan de sparas
type: docs
weight: 10
url: /sv/net/aspose.note.saving/saveoptions/fontssubsystem/
---
## SaveOptions.FontsSubsystem property

Hämtar eller ställer in teckensnittets inställningar som ska användas medan de sparas

```csharp
public FontsSubsystem FontsSubsystem { get; set; }
```

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

Visar hur man sparar ett dokument i pdf-format med standardteckensnitt från en fil.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Spara dokumentet som PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

Visar hur man sparar ett dokument i pdf-format med standardteckensnitt från en ström.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Spara dokumentet som PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### Se även

* class [FontsSubsystem](../../../aspose.note.fonts/fontssubsystem/)
* class [SaveOptions](../)
* namnutrymme [Aspose.Note.Saving](../../saveoptions/)
* hopsättning [Aspose.Note](../../../)


