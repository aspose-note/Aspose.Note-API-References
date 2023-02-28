---
title: Class DocumentFontsSubsystem
second_title: Aspose.Note för .NET API-referens
description: Aspose.Note.Fonts.DocumentFontsSubsystem klass. Enkel implementering av Aspose.Note.Fonts.FontsSubsystem. HämtarFontFamily objekt från OS.
type: docs
weight: 100
url: /sv/net/aspose.note.fonts/documentfontssubsystem/
---
## DocumentFontsSubsystem class

Enkel implementering av Aspose.Note.Fonts.FontsSubsystem. HämtarFontFamily objekt från OS.

```csharp
public class DocumentFontsSubsystem : FontsSubsystem
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor)(Dictionary&lt;string, string&gt;) | Initierar en ny instans av`DocumentFontsSubsystem` class. |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor_1)(Stream, Dictionary&lt;string, string&gt;) | Initierar en ny instans av`DocumentFontsSubsystem` class. |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor_2)(string, Dictionary&lt;string, string&gt;) | Initierar en ny instans av`DocumentFontsSubsystem` class. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| static [Default](../../aspose.note.fonts/documentfontssubsystem/default/) { get; set; } | Hämtar eller ställer in den statiska standardinstansen. |
| [DefaultFont](../../aspose.note.fonts/fontssubsystem/defaultfont/) { get; } | Hämtar eller ställer in standardteckensnitt. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| static [UsingDefaultFont](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfont/)(string, Dictionary&lt;string, string&gt;) | Skapa ny DocumentFontsSubsystem-instans med det angivna standardteckensnittsnamnet. |
| static [UsingDefaultFontFromFile](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/)(string, Dictionary&lt;string, string&gt;) | Skapa ny DocumentFontsSubsystem-instans med ett typsnitt från angiven fil som standard. |
| static [UsingDefaultFontFromStream](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream/)(Stream, Dictionary&lt;string, string&gt;) | Skapa ny DocumentFontsSubsystem-instans med ett teckensnitt från angiven ström som standard. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(Stream) | Lägg till typsnittet. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(string) | Lägg till typsnittet. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(Stream, string) | Lägg till typsnittet. |
| [AddFontSubstitution](../../aspose.note.fonts/fontssubsystem/addfontsubstitution/)(string, string) | Lägger till teckensnittsersättning. |
| virtual [GetFontFamily](../../aspose.note.fonts/fontssubsystem/getfontfamily/)(string) | Får teckensnittsfamilj. |
| [LoadFontsFromFolder](../../aspose.note.fonts/fontssubsystem/loadfontsfromfolder/)(string) | Laddar alla TrueType-teckensnitt från angiven mapp till intern samling. |

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

* class [FontsSubsystem](../fontssubsystem/)
* namnutrymme [Aspose.Note.Fonts](../../aspose.note.fonts/)
* hopsättning [Aspose.Note](../../)


