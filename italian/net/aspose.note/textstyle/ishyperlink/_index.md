---
title: TextStyle.IsHyperlink
second_title: Aspose.Note per .NET API Reference
description: Proprietà TextStyle. Obsoleto dalla versione 22.5. Usare HyperlinkAddress al suo posto.
type: docs
weight: 80
url: /it/net/aspose.note/textstyle/ishyperlink/
---
## TextStyle.IsHyperlink property

Obsoleto dalla versione 22.5. Usare `HyperlinkAddress` al suo posto.

```csharp
public bool IsHyperlink { get; set; }
```

### Esempi

Mostra come associare un collegamento ipertestuale a un testo.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Tasks();

// Crea un oggetto della classe Document
Document doc = new Document();

RichText titleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append("Title!");

Outline outline = new Outline()
                      {
                          MaxWidth = 200,
                          MaxHeight = 200,
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };

TextStyle textStyleRed = new TextStyle
                             {
                                 FontColor = Color.Red,
                                 FontName = "Arial",
                                 FontSize = 10,
                             };

TextStyle textStyleHyperlink = new TextStyle
                                   {
                                       HyperlinkAddress = "https://www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// Aggiungi elementi di contorno
outline.AppendChildLast(outlineElem);

// Inizializza l'oggetto della classe Title
Title title = new Title() { TitleText = titleText };

// Inizializza l'oggetto della classe Page
Page page = new Note.Page() { Title = title };

// Aggiungi nodo Struttura
page.AppendChildLast(outline);

// Aggiungi nodo Pagina
doc.AppendChildLast(page);

// Salva documento OneNote
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

### Guarda anche

* class [TextStyle](../)
* spazio dei nomi [Aspose.Note](../../textstyle/)
* assemblea [Aspose.Note](../../../)


