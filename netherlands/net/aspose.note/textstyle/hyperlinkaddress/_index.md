---
title: TextStyle.HyperlinkAddress
second_title: Aspose.Note voor .NET API-referentie
description: TextStyle eigendom. Haalt of stelt het hyperlinkadres in. Moet worden ingesteld als de waarde van deIsHyperlink eigenschap is waar.
type: docs
weight: 60
url: /nl/net/aspose.note/textstyle/hyperlinkaddress/
---
## TextStyle.HyperlinkAddress property

Haalt of stelt het hyperlinkadres in. Moet worden ingesteld als de waarde van de[`IsHyperlink`](../ishyperlink/) eigenschap is waar.

```csharp
public string HyperlinkAddress { get; set; }
```

### Voorbeelden

Laat zien hoe u een hyperlink aan een tekst koppelt.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Tasks();

// Maak een object van de klasse Document
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
                                       IsHyperlink = true,
                                       HyperlinkAddress = "www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// Voeg overzichtselementen toe
outline.AppendChildLast(outlineElem);

// Initialiseer het titelklasse-object
Title title = new Title() { TitleText = titleText };

// Initialiseer het paginaklasse-object
Page page = new Note.Page() { Title = title };

// Overzichtsknooppunt toevoegen
page.AppendChildLast(outline);

// Paginaknooppunt toevoegen
doc.AppendChildLast(page);

// Sla OneNote-document op
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

### Zie ook

* class [TextStyle](../)
* naamruimte [Aspose.Note](../../textstyle/)
* montage [Aspose.Note](../../../)


