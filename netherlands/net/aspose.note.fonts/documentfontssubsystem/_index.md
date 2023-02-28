---
title: Class DocumentFontsSubsystem
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.Fonts.DocumentFontsSubsystem klas. Eenvoudige implementatie van Aspose.Note.Fonts.FontsSubsystem. Haalt opFontFamily object van OS.
type: docs
weight: 100
url: /nl/net/aspose.note.fonts/documentfontssubsystem/
---
## DocumentFontsSubsystem class

Eenvoudige implementatie van Aspose.Note.Fonts.FontsSubsystem. Haalt opFontFamily object van OS.

```csharp
public class DocumentFontsSubsystem : FontsSubsystem
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor)(Dictionary&lt;string, string&gt;) | Initialiseert een nieuw exemplaar van het`DocumentFontsSubsystem` klasse. |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor_1)(Stream, Dictionary&lt;string, string&gt;) | Initialiseert een nieuw exemplaar van het`DocumentFontsSubsystem` klasse. |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor_2)(string, Dictionary&lt;string, string&gt;) | Initialiseert een nieuw exemplaar van het`DocumentFontsSubsystem` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| static [Default](../../aspose.note.fonts/documentfontssubsystem/default/) { get; set; } | Haalt de statische standaardinstantie op of stelt deze in. |
| [DefaultFont](../../aspose.note.fonts/fontssubsystem/defaultfont/) { get; } | Standaardlettertype ophalen of instellen. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| static [UsingDefaultFont](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfont/)(string, Dictionary&lt;string, string&gt;) | Maak een nieuwe DocumentFontsSubsystem-instantie met de opgegeven standaardlettertypenaam. |
| static [UsingDefaultFontFromFile](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/)(string, Dictionary&lt;string, string&gt;) | Maak een nieuwe DocumentFontsSubsystem-instantie met standaard een lettertype uit het opgegeven bestand. |
| static [UsingDefaultFontFromStream](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream/)(Stream, Dictionary&lt;string, string&gt;) | Maak een nieuwe DocumentFontsSubsystem-instantie met standaard een lettertype uit de opgegeven stream. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(Stream) | Voeg het lettertype toe. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(string) | Voeg het lettertype toe. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(Stream, string) | Voeg het lettertype toe. |
| [AddFontSubstitution](../../aspose.note.fonts/fontssubsystem/addfontsubstitution/)(string, string) | Voegt lettertypevervanging toe. |
| virtual [GetFontFamily](../../aspose.note.fonts/fontssubsystem/getfontfamily/)(string) | Krijgt lettertypefamilie. |
| [LoadFontsFromFolder](../../aspose.note.fonts/fontssubsystem/loadfontsfromfolder/)(string) | Laadt alle TrueType-lettertypen uit de opgegeven map naar de interne verzameling. |

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

* class [FontsSubsystem](../fontssubsystem/)
* naamruimte [Aspose.Note.Fonts](../../aspose.note.fonts/)
* montage [Aspose.Note](../../)


