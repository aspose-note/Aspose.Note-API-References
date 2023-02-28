---
title: Image.Tags
second_title: Aspose.Note per .NET API Reference
description: Image proprietà. Ottiene lelenco di tutti i tag di un paragrafo.
type: docs
weight: 160
url: /it/net/aspose.note/image/tags/
---
## Image.Tags property

Ottiene l'elenco di tutti i tag di un paragrafo.

```csharp
public List<ITag> Tags { get; }
```

### Esempi

Mostra come aggiungere una nuova immagine con tag.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Tags();

// Crea un oggetto della classe Document
Document doc = new Document();

// Inizializza l'oggetto della classe Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inizializza l'oggetto della classe Outline
Outline outline = new Outline(doc);

// Inizializza l'oggetto della classe OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Carica un'immagine
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

// Inserisci l'immagine nel nodo del documento
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// Aggiungi nodo elemento contorno
outline.AppendChildLast(outlineElem);

// Aggiungi nodo di contorno
page.AppendChildLast(outline);

// Aggiungi il nodo della pagina
doc.AppendChildLast(page);

// Salva documento OneNote
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
```

### Guarda anche

* interface [ITag](../../itag/)
* class [Image](../)
* spazio dei nomi [Aspose.Note](../../image/)
* assemblea [Aspose.Note](../../../)


