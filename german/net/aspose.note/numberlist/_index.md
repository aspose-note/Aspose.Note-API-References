---
title: Class NumberList
second_title: Aspose.Note für .NET-API-Referenz
description: Aspose.Note.NumberList klas. Repräsentiert die nummerierte oder Aufzählungsliste.
type: docs
weight: 440
url: /de/net/aspose.note/numberlist/
---
## NumberList class

Repräsentiert die nummerierte oder Aufzählungsliste.

```csharp
public class NumberList
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [NumberList](numberlist/#constructor_1)(string, string, int) | Initialisiert eine neue Instanz von`NumberList`class. Diese Instanz repräsentiert eine Liste mit Aufzählungszeichen. |
| [NumberList](numberlist/#constructor)(string, NumberFormat, string, int) | Initialisiert eine neue Instanz von`NumberList` class. Diese Instanz repräsentiert eine nummerierte Liste. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Font](../../aspose.note/numberlist/font/) { get; set; } | Ruft den Namen der Schriftart ab oder legt ihn fest. |
| [FontColor](../../aspose.note/numberlist/fontcolor/) { get; set; } | Ruft die Schriftfarbe ab oder legt sie fest. |
| [FontSize](../../aspose.note/numberlist/fontsize/) { get; set; } | Ruft die Schriftgröße ab oder legt sie fest. |
| [Format](../../aspose.note/numberlist/format/) { get; set; } | Holt oder setzt das Format des Zeilenkopfes. Für Listen mit Aufzählungszeichen steht ein Aufzählungszeichen. |
| [IsBold](../../aspose.note/numberlist/isbold/) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob der Textstil fett ist. |
| [IsItalic](../../aspose.note/numberlist/isitalic/) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob der Textstil kursiv ist. |
| [LastModifiedTime](../../aspose.note/numberlist/lastmodifiedtime/) { get; set; } | Ruft die letzte Änderungszeit ab oder setzt sie. |
| [NumberFormat](../../aspose.note/numberlist/numberformat/) { get; set; } | Ruft das Zahlenformat ab oder legt es fest, das für eine Gruppe automatisch nummerierter Objekte verwendet wird. Sollte für Listen mit Aufzählungszeichen null sein. |
| [Restart](../../aspose.note/numberlist/restart/) { get; set; } | Ruft den numerischen Wert ab oder legt ihn fest, der den automatischen Zahlenwert des Listenelements überschreibt. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Equals](../../aspose.note/numberlist/equals/#equals)(NumberList) | Bestimmt, ob das angegebene Objekt gleich dem aktuellen Objekt ist. |
| override [Equals](../../aspose.note/numberlist/equals/#equals_1)(object) | Bestimmt, ob das angegebene Objekt gleich dem aktuellen Objekt ist. |
| override [GetHashCode](../../aspose.note/numberlist/gethashcode/)() | dient als Hash-Funktion für den Typ. |
| [GetNumberedListHeader](../../aspose.note/numberlist/getnumberedlistheader/)(int) | Ruft den Kopf der nummerierten Liste ab. |

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

* namensraum [Aspose.Note](../../aspose.note/)
* Montage [Aspose.Note](../../)


