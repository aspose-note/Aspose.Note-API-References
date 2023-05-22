---
title: PdfSaveOptions.JpegQuality
second_title: Aspose.Note for .NET API Reference
description: PdfSaveOptions property. Gets or sets a value determining the quality of the JPEG images inside PDF document. The value may vary from 0 to 100 where 0 means worst quality but maximum compression and 100 means best quality but minimum compression
type: docs
weight: 30
url: /net/aspose.note.saving/pdfsaveoptions/jpegquality/
---
## PdfSaveOptions.JpegQuality property

Gets or sets a value determining the quality of the JPEG images inside PDF document. The value may vary from 0 to 100 where 0 means worst quality but maximum compression and 100 means best quality but minimum compression.

```csharp
public int JpegQuality { get; set; }
```

## Remarks

The default value is 90.

## Examples

Shows how to save a document in pdf format using specific settings.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Initialize PdfSaveOptions object
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Use Jpeg compression
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Quality for JPEG compression
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

### See Also

* class [PdfSaveOptions](../)
* namespace [Aspose.Note.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Note](../../../)


