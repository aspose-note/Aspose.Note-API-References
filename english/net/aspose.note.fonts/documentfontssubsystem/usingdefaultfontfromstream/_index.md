---
title: UsingDefaultFontFromStream
second_title: Aspose.Note for .NET API Reference
description: Create new DocumentFontsSubsystem instance using a font from specified stream as default.
type: docs
weight: 50
url: /net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream/
---
## DocumentFontsSubsystem.UsingDefaultFontFromStream method

Create new DocumentFontsSubsystem instance using a font from specified stream as default.

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromStream(Stream defaultFontStream, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| defaultFontStream | Stream | The stream containing the default font name. |
| fontsSubstitutions | Dictionary`2 | The fonts substitutions. |

### Return Value

The [`DocumentFontsSubsystem`](../../documentfontssubsystem).

### Examples

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

* class [DocumentFontsSubsystem](../../documentfontssubsystem)
* namespace [Aspose.Note.Fonts](../../documentfontssubsystem)
* assembly [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
