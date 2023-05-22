---
title: DocumentFontsSubsystem.UsingDefaultFontFromFile
second_title: Aspose.Note for .NET API Reference
description: DocumentFontsSubsystem method. Create new DocumentFontsSubsystem instance using a font from specified file as default
type: docs
weight: 40
url: /net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/
---
## DocumentFontsSubsystem.UsingDefaultFontFromFile method

Create new DocumentFontsSubsystem instance using a font from specified file as default.

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromFile(string filePath, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| filePath | String | The file containing default font name. |
| fontsSubstitutions | Dictionary`2 | The fonts substitutions. |

### Return Value

The [`DocumentFontsSubsystem`](../).

## Examples

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

### See Also

* class [DocumentFontsSubsystem](../)
* namespace [Aspose.Note.Fonts](../../documentfontssubsystem/)
* assembly [Aspose.Note](../../../)


