---
title: Document.DetectLayoutChanges
second_title: Aspose.Note voor .NET API-referentie
description: Document methode. Detecteert alle wijzigingen die sinds de vorige in de documentlayout zijn aangebrachtDetectLayoutChanges bel. Voor het geval datAutomaticLayoutChangesDetectionEnabled ingesteld op waar automatisch gebruikt bij het begin van documentexport.
type: docs
weight: 90
url: /nl/net/aspose.note/document/detectlayoutchanges/
---
## Document.DetectLayoutChanges method

Detecteert alle wijzigingen die sinds de vorige in de documentlay-out zijn aangebracht`DetectLayoutChanges` bel. Voor het geval dat[`AutomaticLayoutChangesDetectionEnabled`](../automaticlayoutchangesdetectionenabled/) ingesteld op waar, automatisch gebruikt bij het begin van documentexport.

```csharp
public void DetectLayoutChanges()
```

### Voorbeelden

Laat zien hoe u een document in verschillende indelingen kunt opslaan.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initialiseer het nieuwe document
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// Initialiseer de nieuwe pagina
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Standaardstijl voor alle tekst in het document.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Paginaknooppunt toevoegen
doc.AppendChildLast(page);

// Bewaar OneNote-document in verschillende formaten, stel de lettergrootte van tekst in en detecteer lay-outwijzigingen handmatig.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

### Zie ook

* class [Document](../)
* naamruimte [Aspose.Note](../../document/)
* montage [Aspose.Note](../../../)


