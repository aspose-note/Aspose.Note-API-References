---
title: Image.HyperlinkUrl
second_title: Aspose.Note per .NET API Reference
description: Image proprietà. Ottiene o imposta il collegamento ipertestuale associato allimmagine.
type: docs
weight: 110
url: /it/net/aspose.note/image/hyperlinkurl/
---
## Image.HyperlinkUrl property

Ottiene o imposta il collegamento ipertestuale associato all'immagine.

```csharp
public string HyperlinkUrl { get; set; }
```

### Esempi

Mostra come associare un collegamento ipertestuale a un'immagine.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://image.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

### Guarda anche

* class [Image](../)
* spazio dei nomi [Aspose.Note](../../image/)
* assemblea [Aspose.Note](../../../)


