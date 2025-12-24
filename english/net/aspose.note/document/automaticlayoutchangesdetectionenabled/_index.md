---
title: Document.AutomaticLayoutChangesDetectionEnabled
second_title: Aspose.Note for .NET API Reference
description: Document property. Gets or sets a value indicating whether Aspose.Note performs detection of layout changes automatically. Default value is true
type: docs
weight: 20
url: /net/aspose.note/document/automaticlayoutchangesdetectionenabled/
---
## Document.AutomaticLayoutChangesDetectionEnabled property

Gets or sets a value indicating whether Aspose.Note performs detection of layout changes automatically. Default value is `true`.

```csharp
public bool AutomaticLayoutChangesDetectionEnabled { get; set; }
```

## Examples

Shows how to save a document in different formats.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initialize the new Document
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// Initialize the new Page
Page page = new Page();

// Default style for all text in the document.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// Append page node
doc.AppendChildLast(page);

// Save OneNote document in different formats, set text font size and detect layout changes manually.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

### See Also

* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)


