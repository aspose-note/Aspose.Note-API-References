---
title: Image.AlternativeTextDescription
second_title: Aspose.Note per .NET API Reference
description: Image proprietà. Ottiene o imposta un corpo come testo alternativo per limmagine.
type: docs
weight: 30
url: /it/net/aspose.note/image/alternativetextdescription/
---
## Image.AlternativeTextDescription property

Ottiene o imposta un corpo come testo alternativo per l'immagine.

```csharp
public string AlternativeTextDescription { get; set; }
```

### Esempi

Mostra come impostare la descrizione del testo per un'immagine.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Images();

var document = new Document();
var page = new Page(document);
var image = new Image(document, dataDir + "image.jpg")
            {
                AlternativeTextTitle = "This is an image's title!",
                AlternativeTextDescription = "And this is an image's description!"
            };
page.AppendChildLast(image);
document.AppendChildLast(page);

dataDir = dataDir + "ImageAlternativeText_out.one";
document.Save(dataDir);
```

### Guarda anche

* class [Image](../)
* spazio dei nomi [Aspose.Note](../../image/)
* assemblea [Aspose.Note](../../../)


