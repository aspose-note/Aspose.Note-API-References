---
title: Document.AutomaticLayoutChangesDetectionEnabled
second_title: Aspose.Note für .NET-API-Referenz
description: Document eigendom. Ruft einen Wert ab oder legt einen Wert fest der angibt ob Aspose.Note die Erkennung von Layoutänderungen automatisch durchführt. Der Standardwert istWAHR .
type: docs
weight: 20
url: /de/net/aspose.note/document/automaticlayoutchangesdetectionenabled/
---
## Document.AutomaticLayoutChangesDetectionEnabled property

Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob Aspose.Note die Erkennung von Layoutänderungen automatisch durchführt. Der Standardwert ist`WAHR` .

```csharp
public bool AutomaticLayoutChangesDetectionEnabled { get; set; }
```

### Beispiele

Zeigt, wie ein Dokument in verschiedenen Formaten gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Das neue Dokument initialisieren
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// Neue Seite initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Standardstil für den gesamten Text im Dokument.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Seitenknoten anhängen
doc.AppendChildLast(page);

// OneNote-Dokument in verschiedenen Formaten speichern, Textschriftgröße festlegen und Layoutänderungen manuell erkennen.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

### Siehe auch

* class [Document](../)
* namensraum [Aspose.Note](../../document/)
* Montage [Aspose.Note](../../../)


