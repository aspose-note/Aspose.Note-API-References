---
title: Document.DetectLayoutChanges
second_title: Aspose.Note per .NET API Reference
description: Document metodo. Rileva tutte le modifiche apportate al layout del documento dalla precedenteDetectLayoutChanges chiama. Nel casoAutomaticLayoutChangesDetectionEnabled impostato su true utilizzato automaticamente allinizio dellesportazione del documento.
type: docs
weight: 90
url: /it/net/aspose.note/document/detectlayoutchanges/
---
## Document.DetectLayoutChanges method

Rileva tutte le modifiche apportate al layout del documento dalla precedente`DetectLayoutChanges` chiama. Nel caso[`AutomaticLayoutChangesDetectionEnabled`](../automaticlayoutchangesdetectionenabled/) impostato su true, utilizzato automaticamente all'inizio dell'esportazione del documento.

```csharp
public void DetectLayoutChanges()
```

### Esempi

Mostra come salvare un documento in diversi formati.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Inizializza il nuovo documento
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// Inizializza la nuova pagina
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Stile predefinito per tutto il testo nel documento.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Aggiungi il nodo della pagina
doc.AppendChildLast(page);

// Salva il documento OneNote in diversi formati, imposta la dimensione del carattere del testo e rileva manualmente le modifiche al layout.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

### Guarda anche

* class [Document](../)
* spazio dei nomi [Aspose.Note](../../document/)
* assemblea [Aspose.Note](../../../)


