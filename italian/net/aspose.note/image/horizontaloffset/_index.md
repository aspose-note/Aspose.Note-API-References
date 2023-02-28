---
title: Image.HorizontalOffset
second_title: Aspose.Note per .NET API Reference
description: Image proprietà. Ottiene o imposta loffset orizzontale.
type: docs
weight: 100
url: /it/net/aspose.note/image/horizontaloffset/
---
## Image.HorizontalOffset property

Ottiene o imposta l'offset orizzontale.

```csharp
public float HorizontalOffset { get; set; }
```

### Esempi

Mostra come aggiungere un'immagine da un file a un documento con proprietà definite dall'utente.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Images();

// Carica il documento dal flusso.
Document doc = new Document(dataDir + "Aspose.one");

// Ottieni la prima pagina del documento.
Aspose.Note.Page page = doc.FirstChild;

// Carica un'immagine dal file.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Modifica le dimensioni dell'immagine in base alle tue esigenze (opzionale).
                              Width = 100,
                              Height = 100,

                              // Imposta la posizione dell'immagine nella pagina (opzionale).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // Imposta l'allineamento dell'immagine
                              Alignment = HorizontalAlignment.Right
                          };

// Aggiungi l'immagine alla pagina.
page.AppendChildLast(image);
```

### Guarda anche

* class [Image](../)
* spazio dei nomi [Aspose.Note](../../image/)
* assemblea [Aspose.Note](../../../)


