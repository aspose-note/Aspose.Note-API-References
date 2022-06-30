---
title: DocumentFontsSubsystem
second_title: Aspose.Note for .NET API Reference
description: Simple implementation of Aspose.Note.Fonts.FontsSubsystem. Retrieves FontFamily object from OS.
type: docs
weight: 100
url: /net/aspose.note.fonts/documentfontssubsystem/
---
## DocumentFontsSubsystem class

Simple implementation of Aspose.Note.Fonts.FontsSubsystem. Retrieves FontFamily object from OS.

```csharp
public class DocumentFontsSubsystem : FontsSubsystem
```

## Constructors

| Name | Description |
| --- | --- |
| [DocumentFontsSubsystem](documentfontssubsystem#constructor)(Dictionary&lt;string, string&gt;) | Initializes a new instance of the [`DocumentFontsSubsystem`](../documentfontssubsystem) class. |
| [DocumentFontsSubsystem](documentfontssubsystem#constructor_1)(Stream, Dictionary&lt;string, string&gt;) | Initializes a new instance of the [`DocumentFontsSubsystem`](../documentfontssubsystem) class. |
| [DocumentFontsSubsystem](documentfontssubsystem#constructor_2)(string, Dictionary&lt;string, string&gt;) | Initializes a new instance of the [`DocumentFontsSubsystem`](../documentfontssubsystem) class. |

## Properties

| Name | Description |
| --- | --- |
| static [Default](../../aspose.note.fonts/documentfontssubsystem/default) { get; set; } | Gets or sets the static default instance. |
| [DefaultFont](../../aspose.note.fonts/fontssubsystem/defaultfont) { get; } | Gets or sets default font. |

## Methods

| Name | Description |
| --- | --- |
| static [UsingDefaultFont](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfont)(string, Dictionary&lt;string, string&gt;) | Create new DocumentFontsSubsystem instance using specified default font name. |
| static [UsingDefaultFontFromFile](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile)(string, Dictionary&lt;string, string&gt;) | Create new DocumentFontsSubsystem instance using a font from specified file as default. |
| static [UsingDefaultFontFromStream](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream)(Stream, Dictionary&lt;string, string&gt;) | Create new DocumentFontsSubsystem instance using a font from specified stream as default. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont)(Stream) | Add the font. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont)(string) | Add the font. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont)(Stream, string) | Add the font. |
| [AddFontSubstitution](../../aspose.note.fonts/fontssubsystem/addfontsubstitution)(string, string) | Adds font substitution. |
| virtual [GetFontFamily](../../aspose.note.fonts/fontssubsystem/getfontfamily)(string) | Gets font family. |
| [LoadFontsFromFolder](../../aspose.note.fonts/fontssubsystem/loadfontsfromfolder)(string) | Loads all TrueType fonts from specified folder to internal collection. |

### Examples

Shows how to save a document in pdf format using specified default font.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Save the document as PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

Shows how to save a document in pdf format using default font from a file.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Load the document into Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Save the document as PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

Shows how to save a document in pdf format using default font from a stream.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Load the document into Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Save the document as PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### See Also

* class [FontsSubsystem](../fontssubsystem)
* namespace [Aspose.Note.Fonts](../../aspose.note.fonts)
* assembly [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
