---
title: Document.DetectLayoutChanges
second_title: Aspose.Note för .NET API-referens
description: Document metod. Upptäcker alla ändringar som gjorts i dokumentlayouten sedan föregåendeDetectLayoutChanges ring. I fallAutomaticLayoutChangesDetectionEnabled inställd på sant används automatiskt i början av dokumentexporten.
type: docs
weight: 90
url: /sv/net/aspose.note/document/detectlayoutchanges/
---
## Document.DetectLayoutChanges method

Upptäcker alla ändringar som gjorts i dokumentlayouten sedan föregående`DetectLayoutChanges` ring. I fall[`AutomaticLayoutChangesDetectionEnabled`](../automaticlayoutchangesdetectionenabled/) inställd på sant, används automatiskt i början av dokumentexporten.

```csharp
public void DetectLayoutChanges()
```

### Exempel

Visar hur man sparar ett dokument i olika format.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initiera det nya dokumentet
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// Initiera den nya sidan
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Standardstil för all text i dokumentet.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Lägg till sidnod
doc.AppendChildLast(page);

// Spara OneNote-dokument i olika format, ställ in textstorlek och upptäck layoutändringar manuellt.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

### Se även

* class [Document](../)
* namnutrymme [Aspose.Note](../../document/)
* hopsättning [Aspose.Note](../../../)


