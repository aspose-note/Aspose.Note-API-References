---
title: NumberList
second_title: Aspose.Note für .NET-API-Referenz
description: Ruft den Stil für die Überschrift der nummerierten Liste ab oder legt ihn fest.
type: docs
weight: 50
url: /de/net/aspose.note/outlineelement/numberlist/
---
## OutlineElement.NumberList property

Ruft den Stil für die Überschrift der nummerierten Liste ab oder legt ihn fest.

```csharp
public NumberList NumberList { get; set; }
```

### Beispiele

Zeigt, wie Informationen zur Formatierung von Listen abgerufen werden.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// Sammlungsknoten des Gliederungselements abrufen
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// Durch jeden Knoten iterieren
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // Schriftartnamen abrufen
        Console.WriteLine("Font Name: " + list.Font);

        // Schriftlänge abrufen
        Console.WriteLine("Font Length: " + list.Font.Length);

        // Schriftgröße abrufen
        Console.WriteLine("Font Size: " + list.FontSize);

        // Schriftfarbe abrufen
        Console.WriteLine("Font Color: " + list.FontColor);

        // Format abrufen
        Console.WriteLine("Font format: " + list.Format);

        // Fett markieren
        Console.WriteLine("Is bold: " + list.IsBold);

        // Kursiv prüfen
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

Zeigt, wie eine neue Liste mit chinesischer Nummerierung eingefügt wird.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// OneNote-Dokument initialisieren
Aspose.Note.Document doc = new Aspose.Note.Document();

// OneNote-Seite initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// Textstileinstellungen anwenden
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Zahlen in derselben Gliederung werden automatisch erhöht.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

//------------------------
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

//------------------------
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

//------------------------
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// OneNote-Dokument speichern
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

Zeigt, wie neue Listen mit Aufzählungszeichen eingefügt werden.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Erstellen Sie ein Objekt der Document-Klasse
Aspose.Note.Document doc = new Aspose.Note.Document();

// Seitenklassenobjekt initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline-Klassenobjekt initialisieren
Outline outline = new Outline(doc);

// TextStyle-Klassenobjekt initialisieren und Formatierungseigenschaften festlegen
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Objekte der OutlineElement-Klasse initialisieren und Aufzählungszeichen anwenden
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// RichText-Klassenobjekt initialisieren und Textstil anwenden
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Gliederungselemente hinzufügen
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Outline-Knoten hinzufügen
page.AppendChildLast(outline);
// Seitenknoten hinzufügen
doc.AppendChildLast(page);

// OneNote-Dokument speichern
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

Zeigt, wie eine neue Liste mit Nummerierung eingefügt wird.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Erstellen Sie ein Objekt der Document-Klasse
Document doc = new Document();

// Seitenklassenobjekt initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline-Klassenobjekt initialisieren
Outline outline = new Outline(doc);

// TextStyle-Klassenobjekt initialisieren und Formatierungseigenschaften festlegen
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Objekte der OutlineElement-Klasse initialisieren und Nummerierung anwenden
// Zahlen in derselben Gliederung werden automatisch erhöht.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Gliederungselemente hinzufügen
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Outline-Knoten hinzufügen
page.AppendChildLast(outline);

// Seitenknoten hinzufügen
doc.AppendChildLast(page);

// OneNote-Dokument speichern
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

### Siehe auch

* class [NumberList](../../numberlist)
* class [OutlineElement](../../outlineelement)
* namensraum [Aspose.Note](../../outlineelement)
* Montage [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
