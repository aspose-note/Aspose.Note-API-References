---
title: DocumentFontsSubsystem.UsingDefaultFont
second_title: Aspose.Note for .NET API Reference
description: DocumentFontsSubsystem method. Create new DocumentFontsSubsystem instance using specified default font name
type: docs
weight: 30
url: /net/aspose.note.fonts/documentfontssubsystem/usingdefaultfont/
---
## DocumentFontsSubsystem.UsingDefaultFont method

Create new DocumentFontsSubsystem instance using specified default font name.

```csharp
public static DocumentFontsSubsystem UsingDefaultFont(string defaultFontName, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| defaultFontName | String | The default font name. |
| fontsSubstitutions | Dictionary`2 | The fonts substitutions. |

### Return Value

The [`DocumentFontsSubsystem`](../).

## Examples

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

### See Also

* class [DocumentFontsSubsystem](../)
* namespace [Aspose.Note.Fonts](../../documentfontssubsystem/)
* assembly [Aspose.Note](../../../)


