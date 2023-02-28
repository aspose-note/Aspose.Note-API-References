---
title: Class RichText
second_title: Aspose.Note für .NET-API-Referenz
description: Aspose.Note.RichText klas. Stellt einen RichText dar.
type: docs
weight: 530
url: /de/net/aspose.note/richtext/
---
## RichText class

Stellt einen Rich-Text dar.

```csharp
public sealed class RichText : Node, IEnumerable<char>, IOutlineElementChildNode, ITaggable
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [RichText](richtext/#constructor)() | Initialisiert eine neue Instanz von`RichText` Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Alignment](../../aspose.note/richtext/alignment/) { get; set; } | Ruft die Ausrichtung ab oder legt sie fest. |
| [Document](../../aspose.note/node/document/) { get; } | Ruft das Dokument des Knotens ab. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | Ruft einen Wert ab, der angibt, ob dieser Knoten zusammengesetzt ist. Wenn wahr, kann der Knoten untergeordnete Knoten haben. |
| [LastModifiedTime](../../aspose.note/richtext/lastmodifiedtime/) { get; set; } | Ruft die letzte Änderungszeit ab oder setzt sie. |
| [Length](../../aspose.note/richtext/length/) { get; } | Ruft die Länge des Textes ab. |
| [LineSpacing](../../aspose.note/richtext/linespacing/) { get; set; } | Ruft den Zeilenabstand ab oder legt ihn fest. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Ruft den nächsten Knoten auf derselben Knotenbaumebene ab. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Ruft den Knotentyp ab. |
| [ParagraphStyle](../../aspose.note/richtext/paragraphstyle/) { get; set; } | Ruft den Absatzstil ab oder legt ihn fest. Diese Einstellungen werden verwendet, wenn kein passendes TextStyle-Objekt vorhanden istStyles entweder dieses Objekt gibt keine erforderliche Einstellung an. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Ruft den übergeordneten Knoten ab. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Ruft den vorherigen Knoten auf derselben Knotenbaumebene ab. |
| [SpaceAfter](../../aspose.note/richtext/spaceafter/) { get; set; } | Ruft den Mindestabstand nach ab oder legt ihn fest. |
| [SpaceBefore](../../aspose.note/richtext/spacebefore/) { get; set; } | Ruft die minimale Menge an Speicherplatz ab oder legt sie fest. |
| [Tags](../../aspose.note/richtext/tags/) { get; } | Ruft die Liste aller Tags eines Absatzes ab. |
| [Text](../../aspose.note/richtext/text/) { get; set; } | Holt oder setzt den Text. Der String DARF KEINE Zeichen des Wertes 10 (Zeilenvorschub) enthalten. |
| [TextRuns](../../aspose.note/richtext/textruns/) { get; } | Ruft die Sammlung von Textläufen ab. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [Accept](../../aspose.note/richtext/accept/)(DocumentVisitor) | Akzeptiert den Besucher des Knotens. |
| [Append](../../aspose.note/richtext/append/#append)(string) | Fügt dem letzten Textbereich eine Zeichenfolge hinzu. |
| [Append](../../aspose.note/richtext/append/#append_1)(string, TextStyle) | Fügt am Ende eine Zeichenfolge hinzu. |
| [AppendFront](../../aspose.note/richtext/appendfront/#appendfront)(string) | Fügt eine Zeichenfolge am Anfang des ersten Textbereichs hinzu. |
| [AppendFront](../../aspose.note/richtext/appendfront/#appendfront_1)(string, TextStyle) | Fügt vorne eine Zeichenfolge hinzu. |
| [Clear](../../aspose.note/richtext/clear/)() | Löscht den Inhalt dieser Instanz. |
| [GetEnumerator](../../aspose.note/richtext/getenumerator/)() | Gibt einen Enumerator zurück, der die Zeichen dieses RichText-Objekts durchläuft. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof)(char) | Gibt den nullbasierten Index des ersten Vorkommens des angegebenen Unicode-Zeichens in dieser Zeichenfolge zurück. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_3)(string) | Gibt den nullbasierten Index des ersten Vorkommens der angegebenen Zeichenfolge in dieser Instanz zurück. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_1)(char, int) | Gibt den nullbasierten Index des ersten Vorkommens des angegebenen Unicode-Zeichens in dieser Zeichenfolge zurück. Die Suche beginnt an einer bestimmten Zeichenposition. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_4)(string, int) | Gibt den nullbasierten Index des ersten Vorkommens der angegebenen Zeichenfolge in dieser Instanz zurück. Die Suche beginnt an einer bestimmten Zeichenposition. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_8)(string, StringComparison) | Gibt den nullbasierten Index des ersten Vorkommens der angegebenen Zeichenfolge in der aktuellen Instanz zurück. Ein Parameter gibt den Suchtyp an, der für die angegebene Zeichenfolge verwendet werden soll. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_2)(char, int, int) | Gibt den nullbasierten Index des ersten Vorkommens des angegebenen Zeichens in dieser Instanz zurück. Die Suche beginnt an einer bestimmten Zeichenposition und untersucht eine bestimmte Anzahl von Zeichenpositionen. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_5)(string, int, int) | Gibt den nullbasierten Index des ersten Vorkommens der angegebenen Zeichenfolge in dieser Instanz zurück. Die Suche beginnt an einer bestimmten Zeichenposition und untersucht eine bestimmte Anzahl von Zeichenpositionen. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_7)(string, int, StringComparison) | Gibt den nullbasierten Index des ersten Vorkommens der angegebenen Zeichenfolge in der aktuellen Instanz zurück. Parameter geben die Startposition der Suche in der aktuellen Zeichenfolge und den Suchtyp an, der für die angegebene Zeichenfolge verwendet werden soll. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_6)(string, int, int, StringComparison) | Gibt den nullbasierten Index des ersten Vorkommens der angegebenen Zeichenfolge in der aktuellen Instanz zurück. |
| [Insert](../../aspose.note/richtext/insert/#insert)(int, string) | Fügt in dieser Instanz eine angegebene Zeichenfolge an einer angegebenen Indexposition ein. |
| [Insert](../../aspose.note/richtext/insert/#insert_1)(int, string, TextStyle) | Fügt eine angegebene Zeichenfolge mit angegebenem Stil an einer angegebenen Indexposition in dieser Instanz ein. |
| [Remove](../../aspose.note/richtext/remove/#remove)(int) | Entfernt alle Zeichen in der aktuellen Instanz, beginnend an einer bestimmten Position und fortgesetzt bis zur letzten Position. |
| [Remove](../../aspose.note/richtext/remove/#remove_1)(int, int) | Entfernt die angegebene Anzahl von Zeichen in der aktuellen Instanz, beginnend an einer angegebenen Position. |
| [Replace](../../aspose.note/richtext/replace/#replace)(char, char) | Ersetzt alle Vorkommen eines angegebenen Unicode-Zeichens in dieser Instanz durch ein anderes angegebenes Unicode-Zeichen. |
| [Replace](../../aspose.note/richtext/replace/#replace_1)(string, string) | Ersetzt alle Vorkommen einer angegebenen Zeichenfolge in der aktuellen Instanz durch eine andere angegebene Zeichenfolge. |
| [Replace](../../aspose.note/richtext/replace/#replace_2)(string, string, TextStyle) | Ersetzt alle Vorkommen einer angegebenen Zeichenfolge in der aktuellen Instanz durch eine andere angegebene Zeichenfolge im angegebenen Stil. |
| [Trim](../../aspose.note/richtext/trim/#trim)() | Entfernt alle führenden und abschließenden Leerzeichen. |
| [Trim](../../aspose.note/richtext/trim/#trim_1)(char) | Entfernt alle führenden und abschließenden Instanzen eines Zeichens. |
| [Trim](../../aspose.note/richtext/trim/#trim_2)(params char[]) | Entfernt alle führenden und nachgestellten Vorkommen einer in einem Array angegebenen Zeichengruppe. |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend)() | Entfernt alle abschließenden Leerzeichen. |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend_1)(char) | Entfernt alle nachfolgenden Vorkommen eines Zeichens. |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend_2)(params char[]) | Entfernt alle nachgestellten Vorkommen einer Reihe von Zeichen, die in einem Array angegeben sind. |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart)() | Entfernt alle führenden Leerzeichen. |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart_1)(char) | Entfernt alle führenden Vorkommen eines angegebenen Zeichens. |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart_2)(params char[]) | Entfernt alle führenden Vorkommen einer Reihe von Zeichen, die in einem Array angegeben sind. |

### Beispiele

Zeigt, wie der gesamte Text aus dem Dokument abgerufen wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Text();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Text abrufen
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// Text auf dem Ausgabebildschirm drucken
Console.WriteLine(text);
```

Zeigt, wie der gesamte Text von der Seite abgerufen wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Text();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Liste der Seitenknoten abrufen
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // Text abrufen
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // Text auf dem Ausgabebildschirm drucken
    Console.WriteLine(text);
}
```

Lassen Sie uns die Seitentitel unter anderen Überschriften hervorheben, indem wir die Schriftgröße erhöhen.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Laden Sie das Dokument in Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Seitentitel durchlaufen.
foreach (var title in document.Select(e => e.Title.TitleText))
{
    title.ParagraphStyle.FontSize = 24;
    title.ParagraphStyle.IsBold = true;

    foreach (var run in title.TextRuns)
    {
        run.Style.FontSize = 24;
        run.Style.IsBold = true;
    }
}

document.Save(Path.Combine(dataDir, "ChangePageTitleStyle.pdf"));
```

Zeigt, wie Text aus jeder Tabellenzeile abgerufen wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Tables();

// Laden Sie das Dokument in Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Holen Sie sich eine Liste von Tabellenknoten
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // Tabellenzeilen durchlaufen
    foreach (TableRow row in table)
    {
        // Text abrufen
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // Text auf dem Ausgabebildschirm drucken
        Console.WriteLine(text);
    }
}
```

Zeigt, wie Text aus einer Tabelle abgerufen wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Tables();

// Laden Sie das Dokument in Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Holen Sie sich eine Liste von Tabellenknoten
IList<Table> nodes = document.GetChildNodes<Table>();

// Tabellenanzahl setzen
int tblCount = 0;

foreach (Table table in nodes)
{
    tblCount++;
    Console.WriteLine("table # " + tblCount);

    // Text abrufen
    string text = string.Join(Environment.NewLine, table.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

    // Text auf dem Ausgabebildschirm drucken
    Console.WriteLine(text);
}
```

Lassen Sie uns die Änderungen des letzten Textes hervorheben, indem wir sie hervorheben.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Laden Sie das Dokument in Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// RichText-Knoten abrufen, die letzte Woche geändert wurden.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // Hervorhebungsfarbe setzen
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // Hervorhebungsfarbe setzen
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

Zeigt, wie Sie einen Titel für eine Seite festlegen.

```csharp
string dataDir = RunExamples.GetDataDir_Text();
string outputPath = dataDir + "CreateTitleMsStyle_out.one";

var doc = new Document();
var page = new Page(doc);

page.Title = new Title(doc)
{
    TitleText = new RichText(doc)
    {
        Text = "Title text.",
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleDate = new RichText(doc)
    {
        Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture),
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleTime = new RichText(doc)
    {
        Text = "12:34",
        ParagraphStyle = ParagraphStyle.Default
    }
};

doc.AppendChildLast(page);

doc.Save(outputPath);
```

Legen Sie die Korrektursprache für einen Text fest.

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = ParagraphStyle.Default };
text.Append("United States", new TextStyle() { Language = CultureInfo.GetCultureInfo("en-US") })
    .Append(" Germany", new TextStyle() { Language = CultureInfo.GetCultureInfo("de-DE") })
    .Append(" China", new TextStyle() { Language = CultureInfo.GetCultureInfo("zh-CN") });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetProofingLanguageForText.one"));
```

Zeigt, wie man alle Seiten durchgeht und eine Ersetzung im Text vornimmt.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Alle RichText-Knoten abrufen
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Text einer Form ersetzen
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

// In jedem unterstützten Dateiformat speichern
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Bearbeiten nach Textformat mit Absatzstil.

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = new ParagraphStyle() { FontName = "Courier New", FontSize = 20 } }
                .Append($"DefaultParagraphFontAndSize{Environment.NewLine}")
                .Append($"OnlyDefaultParagraphFont{Environment.NewLine}", new TextStyle() { FontSize = 14 })
                .Append("OnlyDefaultParagraphFontSize", new TextStyle() { FontName = "Verdana" });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetDefaultParagraphStyle.one"));
```

Zeigt, wie Text aus den Zellen einer Tabelle abgerufen wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Tables();

// Laden Sie das Dokument in Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Holen Sie sich eine Liste von Tabellenknoten
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // Tabellenzeilen durchlaufen
    foreach (TableRow row in table)
    {
        // Liste der TableCell-Knoten abrufen
        // Durch Tabellenzellen iterieren
        foreach (TableCell cell in row)
        {
            // Text abrufen
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // Text auf dem Ausgabebildschirm drucken
            Console.WriteLine(text);
        }
    }
}
```

Zeigt, wie man den Text der Seite durchläuft und eine Ersetzung vornimmt.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// Alle RichText-Knoten abrufen
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Text einer Form ersetzen
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// In jedem unterstützten Dateiformat speichern
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Zeigt, wie Sie ein Dokument erstellen und es mit Standardoptionen im HTML-Format speichern.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// OneNote-Dokument initialisieren
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

// Standardstil für den gesamten Text im Dokument.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// Im HTML-Format speichern
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

Zeigt, wie man einen neuen Absatz mit Tag hinzufügt.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Tags();

// Erstellen Sie ein Objekt der Document-Klasse
Document doc = new Document();

// Seitenklassenobjekt initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline-Klassenobjekt initialisieren
Outline outline = new Outline(doc);

// OutlineElement-Klassenobjekt initialisieren
OutlineElement outlineElem = new OutlineElement(doc);
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
RichText text = new RichText(doc) { Text = "OneNote text.", ParagraphStyle = textStyle };
text.Tags.Add(NoteTag.CreateYellowStar());

// Textknoten hinzufügen
outlineElem.AppendChildLast(text);

// Gliederungselementknoten hinzufügen
outline.AppendChildLast(outlineElem);

// Gliederungsknoten hinzufügen
page.AppendChildLast(outline);

// Seitenknoten hinzufügen
doc.AppendChildLast(page);

// OneNote-Dokument speichern
dataDir = dataDir + "AddTextNodeWithTag_out.one";
doc.Save(dataDir);
```

Zeigt, wie man ein Dokument erstellt und einen bestimmten Seitenbereich im HTML-Format speichert.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// OneNote-Dokument initialisieren
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Standardstil für den gesamten Text im Dokument.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// Im HTML-Format speichern
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

Zeigt, wie auf die Details eines Tags zugegriffen wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Tags();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "TagFile.one");

// Alle RichText-Knoten abrufen
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Durch jeden Knoten iterieren
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // Eigenschaften abrufen
            Console.WriteLine($"    Completed Time: {noteTag.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTag.CreationTime}");
            Console.WriteLine($"    Font Color: {noteTag.FontColor}");
            Console.WriteLine($"    Status: {noteTag.Status}");
            Console.WriteLine($"    Label: {noteTag.Label}");
            Console.WriteLine($"    Icon: {noteTag.Icon}");
            Console.WriteLine($"    High Light: {noteTag.Highlight}");
        }
    }
}
```

Zeigt, wie ein Dokument mit einem Text erstellt wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Erstellen Sie ein Objekt der Document-Klasse
Document doc = new Document();

// Seitenklassenobjekt initialisieren
Page page = new Page(doc);

// Outline-Klassenobjekt initialisieren
Outline outline = new Outline(doc);

// OutlineElement-Klassenobjekt initialisieren
OutlineElement outlineElem = new OutlineElement(doc);

// TextStyle-Klassenobjekt initialisieren und Formatierungseigenschaften festlegen
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// RichText-Klassenobjekt initialisieren und Textstil anwenden
RichText text = new RichText(doc) { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// RichText-Knoten hinzufügen
outlineElem.AppendChildLast(text);

// OutlineElement-Knoten hinzufügen
outline.AppendChildLast(outlineElem);

// Outline-Knoten hinzufügen
page.AppendChildLast(outline);

// Seitenknoten hinzufügen
doc.AppendChildLast(page);

// OneNote-Dokument speichern
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
doc.Save(dataDir);
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

Zeigt, wie eine Vorlage für ein wöchentliches Meeting vorbereitet wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Tags();

// Erstellen Sie ein Objekt der Document-Klasse
var headerStyle = new ParagraphStyle() { FontName = "Calibri", FontSize = 16 };
var bodyStyle = new ParagraphStyle() { FontName = "Calibri", FontSize = 12 };

var d = new Document();
bool restartFlag = true;
var outline = d.AppendChildLast(new Page()
                                    {
                                        Title = new Title() { TitleText = new RichText() { Text = $"Weekly meeting {DateTime.Today:d}", ParagraphStyle = ParagraphStyle.Default } }
                                    })
               .AppendChildLast(new Outline() { VerticalOffset = 30, HorizontalOffset = 30 });

outline.AppendChildLast(new OutlineElement())
       .AppendChildLast(new RichText() { Text = "Important", ParagraphStyle = headerStyle });
foreach (var e in new[] { "First", "Second", "Third" })
{
    outline.AppendChildLast(new OutlineElement() { NumberList = CreateListNumberingStyle(bodyStyle, restartFlag) })
           .AppendChildLast(new RichText() { Text = e, ParagraphStyle = bodyStyle });
    restartFlag = false;
}

outline.AppendChildLast(new OutlineElement())
       .AppendChildLast(new RichText() { Text = "TO DO", ParagraphStyle = headerStyle, SpaceBefore = 15 });
restartFlag = true;
foreach (var e in new[] { "First", "Second", "Third" })
{
    outline.AppendChildLast(new OutlineElement() { NumberList = CreateListNumberingStyle(bodyStyle, restartFlag) })
           .AppendChildLast(new RichText() { Text = e, ParagraphStyle = bodyStyle, Tags = { NoteCheckBox.CreateBlueCheckBox() } });
    restartFlag = false;
}

d.Save(Path.Combine(dataDir, "meetingNotes.one"));
```

Zeigt, wie ein Hyperlink an einen Text gebunden wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Tasks();

// Erstellen Sie ein Objekt der Document-Klasse
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

// Gliederungselemente hinzufügen
outline.AppendChildLast(outlineElem);

// Titelklassenobjekt initialisieren
Title title = new Title() { TitleText = titleText };

// Seitenklassenobjekt initialisieren
Page page = new Note.Page() { Title = title };

// Outline-Knoten hinzufügen
page.AppendChildLast(outline);

// Seitenknoten hinzufügen
doc.AppendChildLast(page);

// OneNote-Dokument speichern
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

### Siehe auch

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [ITaggable](../itaggable/)
* namensraum [Aspose.Note](../../aspose.note/)
* Montage [Aspose.Note](../../)


