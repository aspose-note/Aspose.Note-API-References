---
title: Class RichText
second_title: Aspose.Note per .NET API Reference
description: Aspose.Note.RichText classe. Rappresenta un rich text.
type: docs
weight: 530
url: /it/net/aspose.note/richtext/
---
## RichText class

Rappresenta un rich text.

```csharp
public sealed class RichText : Node, IEnumerable<char>, IOutlineElementChildNode, ITaggable
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [RichText](richtext/#constructor)() | Inizializza una nuova istanza di`RichText` classe. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Alignment](../../aspose.note/richtext/alignment/) { get; set; } | Ottiene o imposta l'allineamento. |
| [Document](../../aspose.note/node/document/) { get; } | Ottiene il documento del nodo. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | Ottiene un valore che indica se questo nodo è composto. Se vero il nodo può avere nodi figli. |
| [LastModifiedTime](../../aspose.note/richtext/lastmodifiedtime/) { get; set; } | Ottiene o imposta l'ora dell'ultima modifica. |
| [Length](../../aspose.note/richtext/length/) { get; } | Ottiene la lunghezza del testo. |
| [LineSpacing](../../aspose.note/richtext/linespacing/) { get; set; } | Ottiene o imposta l'interlinea. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Ottiene il nodo successivo allo stesso livello di albero dei nodi. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Ottiene il tipo di nodo. |
| [ParagraphStyle](../../aspose.note/richtext/paragraphstyle/) { get; set; } | Ottiene o imposta lo stile di paragrafo. Queste impostazioni vengono utilizzate se non esiste un oggetto TextStyle corrispondente inStyles collection o questo oggetto non specifica un'impostazione necessaria. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Ottiene il nodo padre. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Ottiene il nodo precedente allo stesso livello dell'albero dei nodi. |
| [SpaceAfter](../../aspose.note/richtext/spaceafter/) { get; set; } | Ottiene o imposta la quantità minima di spazio dopo. |
| [SpaceBefore](../../aspose.note/richtext/spacebefore/) { get; set; } | Ottiene o imposta la quantità minima di spazio prima di. |
| [Tags](../../aspose.note/richtext/tags/) { get; } | Ottiene l'elenco di tutti i tag di un paragrafo. |
| [Text](../../aspose.note/richtext/text/) { get; set; } | Ottiene o imposta il testo. La stringa NON DEVE contenere caratteri con valore 10 (line feed). |
| [TextRuns](../../aspose.note/richtext/textruns/) { get; } | Ottiene la raccolta di sequenze di testo. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Accept](../../aspose.note/richtext/accept/)(DocumentVisitor) | Accetta il visitatore del nodo. |
| [Append](../../aspose.note/richtext/append/#append)(string) | Aggiunge una stringa all'ultimo intervallo di testo. |
| [Append](../../aspose.note/richtext/append/#append_1)(string, TextStyle) | Aggiunge una stringa alla fine. |
| [AppendFront](../../aspose.note/richtext/appendfront/#appendfront)(string) | Aggiunge una stringa all'inizio del primo intervallo di testo. |
| [AppendFront](../../aspose.note/richtext/appendfront/#appendfront_1)(string, TextStyle) | Aggiunge una stringa in primo piano. |
| [Clear](../../aspose.note/richtext/clear/)() | Cancella il contenuto di questa istanza. |
| [GetEnumerator](../../aspose.note/richtext/getenumerator/)() | Restituisce un enumeratore che scorre i caratteri di questo oggetto RichText. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof)(char) | Restituisce l'indice in base zero della prima occorrenza del carattere Unicode specificato in questa stringa. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_3)(string) | Restituisce l'indice in base zero della prima occorrenza della stringa specificata in questa istanza. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_1)(char, int) | Restituisce l'indice in base zero della prima occorrenza del carattere Unicode specificato in questa stringa. La ricerca inizia in una posizione di carattere specificata. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_4)(string, int) | Restituisce l'indice in base zero della prima occorrenza della stringa specificata in questa istanza. La ricerca inizia in una posizione di carattere specificata. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_8)(string, StringComparison) | Restituisce l'indice in base zero della prima occorrenza della stringa specificata nell'istanza corrente. Un parametro specifica il tipo di ricerca da utilizzare per la stringa specificata. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_2)(char, int, int) | Restituisce l'indice in base zero della prima occorrenza del carattere specificato in questa istanza. La ricerca inizia da una posizione di carattere specificata ed esamina un numero specificato di posizioni di carattere. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_5)(string, int, int) | Restituisce l'indice in base zero della prima occorrenza della stringa specificata in questa istanza. La ricerca inizia da una posizione di carattere specificata ed esamina un numero specificato di posizioni di carattere. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_7)(string, int, StringComparison) | Restituisce l'indice in base zero della prima occorrenza della stringa specificata nell'istanza corrente. I parametri specificano la posizione iniziale della ricerca nella stringa corrente e il tipo di ricerca da utilizzare per la stringa specificata. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_6)(string, int, int, StringComparison) | Restituisce l'indice in base zero della prima occorrenza della stringa specificata nell'istanza corrente. |
| [Insert](../../aspose.note/richtext/insert/#insert)(int, string) | Inserisce una stringa specificata in una posizione di indice specificata in questa istanza. |
| [Insert](../../aspose.note/richtext/insert/#insert_1)(int, string, TextStyle) | Inserisce una stringa specificata con uno stile specificato in una posizione di indice specificata in questa istanza. |
| [Remove](../../aspose.note/richtext/remove/#remove)(int) | Rimuove tutti i caratteri nell'istanza corrente, iniziando da una posizione specificata e proseguendo fino all'ultima posizione. |
| [Remove](../../aspose.note/richtext/remove/#remove_1)(int, int) | Rimuove il numero specificato di caratteri nell'istanza corrente a partire da una posizione specificata. |
| [Replace](../../aspose.note/richtext/replace/#replace)(char, char) | Sostituisce tutte le occorrenze di un carattere Unicode specificato in questa istanza con un altro carattere Unicode specificato. |
| [Replace](../../aspose.note/richtext/replace/#replace_1)(string, string) | Sostituisce tutte le occorrenze di una stringa specificata nell'istanza corrente con un'altra stringa specificata. |
| [Replace](../../aspose.note/richtext/replace/#replace_2)(string, string, TextStyle) | Sostituisce tutte le occorrenze di una stringa specificata nell'istanza corrente con un'altra stringa specificata nello stile specificato. |
| [Trim](../../aspose.note/richtext/trim/#trim)() | Rimuove tutti gli spazi bianchi iniziali e finali. |
| [Trim](../../aspose.note/richtext/trim/#trim_1)(char) | Rimuove tutte le istanze iniziali e finali di un carattere. |
| [Trim](../../aspose.note/richtext/trim/#trim_2)(params char[]) | Rimuove tutte le occorrenze iniziali e finali di un set di caratteri specificato in un array. |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend)() | Rimuove tutti gli spazi vuoti finali. |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend_1)(char) | Rimuove tutte le occorrenze finali di un carattere. |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend_2)(params char[]) | Rimuove tutte le occorrenze finali di un set di caratteri specificato in un array. |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart)() | Rimuove tutti gli spazi bianchi iniziali. |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart_1)(char) | Rimuove tutte le occorrenze iniziali di un carattere specificato. |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart_2)(params char[]) | Rimuove tutte le occorrenze iniziali di un set di caratteri specificato in un array. |

### Esempi

Mostra come ottenere tutto il testo dal documento.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Text();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Recupera il testo
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// Stampa il testo sullo schermo di output
Console.WriteLine(text);
```

Mostra come ottenere tutto il testo dalla pagina.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Text();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Ottieni l'elenco dei nodi della pagina
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // Recupera il testo
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // Stampa il testo sullo schermo di output
    Console.WriteLine(text);
}
```

Mettiamo in risalto i titoli delle pagine tra le altre intestazioni aumentando la dimensione del carattere.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Carica il documento in Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Itera attraverso i titoli della pagina.
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

Mostra come ottenere il testo da ogni riga della tabella.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Tables();

// Carica il documento in Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Ottieni un elenco di nodi della tabella
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // Itera attraverso le righe della tabella
    foreach (TableRow row in table)
    {
        // Recupera il testo
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // Stampa il testo sullo schermo di output
        Console.WriteLine(text);
    }
}
```

Mostra come ottenere testo da una tabella.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Tables();

// Carica il documento in Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Ottieni un elenco di nodi della tabella
IList<Table> nodes = document.GetChildNodes<Table>();

// Imposta il conteggio della tabella
int tblCount = 0;

foreach (Table table in nodes)
{
    tblCount++;
    Console.WriteLine("table # " + tblCount);

    // Recupera il testo
    string text = string.Join(Environment.NewLine, table.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

    // Stampa il testo sullo schermo di output
    Console.WriteLine(text);
}
```

Sottolineiamo le ultime modifiche al testo evidenziando.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Carica il documento in Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Ottieni i nodi RichText modificati la scorsa settimana.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // Imposta il colore di evidenziazione
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // Imposta il colore di evidenziazione
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

Mostra come impostare un titolo per una pagina.

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

Imposta la lingua di correzione per un testo.

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

Mostra come scorrere tutte le pagine e fare una sostituzione nel testo.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Ottieni tutti i nodi RichText
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Sostituisci il testo di una forma
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

// Salva in qualsiasi formato di file supportato
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Manipolare in base al formato del testo utilizzando lo stile di paragrafo.

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

Mostra come ottenere testo dalle celle di una tabella.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Tables();

// Carica il documento in Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Ottieni un elenco di nodi della tabella
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // Itera attraverso le righe della tabella
    foreach (TableRow row in table)
    {
        // Ottieni l'elenco dei nodi TableCell
        // Itera attraverso le celle della tabella
        foreach (TableCell cell in row)
        {
            // Recupera il testo
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // Stampa il testo sullo schermo di output
            Console.WriteLine(text);
        }
    }
}
```

Mostra come passare attraverso il testo della pagina ed effettuare una sostituzione.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// Ottieni tutti i nodi RichText
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Sostituisci il testo di una forma
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// Salva in qualsiasi formato di file supportato
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Mostra come creare un documento e salvarlo in formato html utilizzando le opzioni predefinite.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Inizializza il documento OneNote
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

// Stile predefinito per tutto il testo nel documento.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// Salva in formato HTML
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

Mostra come aggiungere un nuovo paragrafo con tag.

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
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
RichText text = new RichText(doc) { Text = "OneNote text.", ParagraphStyle = textStyle };
text.Tags.Add(NoteTag.CreateYellowStar());

// Aggiungi nodo di testo
outlineElem.AppendChildLast(text);

// Aggiungi nodo elemento contorno
outline.AppendChildLast(outlineElem);

// Aggiungi nodo di contorno
page.AppendChildLast(outline);

// Aggiungi il nodo della pagina
doc.AppendChildLast(page);

// Salva documento OneNote
dataDir = dataDir + "AddTextNodeWithTag_out.one";
doc.Save(dataDir);
```

Mostra come creare un documento e salvarlo in un intervallo di pagine specificato in formato html.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Inizializza il documento OneNote
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Stile predefinito per tutto il testo nel documento.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// Salva in formato HTML
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

Mostra come accedere ai dettagli di un tag.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Tags();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "TagFile.one");

// Ottieni tutti i nodi RichText
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Itera attraverso ogni nodo
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // Recupera le proprietà
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

Mostra come creare un documento con un testo.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Crea un oggetto della classe Document
Document doc = new Document();

// Inizializza l'oggetto della classe Page
Page page = new Page(doc);

// Inizializza l'oggetto della classe Outline
Outline outline = new Outline(doc);

// Inizializza l'oggetto della classe OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Inizializza l'oggetto della classe TextStyle e imposta le proprietà di formattazione
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Inizializza l'oggetto della classe RichText e applica lo stile del testo
RichText text = new RichText(doc) { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// Aggiungi nodo RichText
outlineElem.AppendChildLast(text);

// Aggiungi nodo OutlineElement
outline.AppendChildLast(outlineElem);

// Aggiungi nodo Struttura
page.AppendChildLast(outline);

// Aggiungi nodo Pagina
doc.AppendChildLast(page);

// Salva documento OneNote
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
doc.Save(dataDir);
```

Mostra come inserire una nuova lista con numerazione cinese.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Inizializza il documento OneNote
Aspose.Note.Document doc = new Aspose.Note.Document();

// Inizializza la pagina di OneNote
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// Applica le impostazioni dello stile del testo
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// I numeri nella stessa struttura vengono incrementati automaticamente.
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

// Salva documento OneNote
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

Mostra come inserire nuovi elenchi puntati.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Crea un oggetto della classe Document
Aspose.Note.Document doc = new Aspose.Note.Document();

// Inizializza l'oggetto della classe Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inizializza l'oggetto della classe Outline
Outline outline = new Outline(doc);

// Inizializza l'oggetto della classe TextStyle e imposta le proprietà di formattazione
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Inizializza gli oggetti della classe OutlineElement e applica i punti elenco
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// Inizializza l'oggetto della classe RichText e applica lo stile del testo
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Aggiungi elementi di contorno
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Aggiungi nodo Struttura
page.AppendChildLast(outline);
// Aggiungi nodo Pagina
doc.AppendChildLast(page);

// Salva documento OneNote
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

Mostra come inserire una nuova lista con numerazione.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Crea un oggetto della classe Document
Document doc = new Document();

// Inizializza l'oggetto della classe Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inizializza l'oggetto della classe Outline
Outline outline = new Outline(doc);

// Inizializza l'oggetto della classe TextStyle e imposta le proprietà di formattazione
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Inizializza gli oggetti della classe OutlineElement e applica la numerazione
// I numeri nella stessa struttura vengono incrementati automaticamente.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Aggiungi elementi di contorno
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Aggiungi nodo Struttura
page.AppendChildLast(outline);

// Aggiungi nodo Pagina
doc.AppendChildLast(page);

// Salva documento OneNote
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

Mostra come preparare un modello per una riunione settimanale.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Tags();

// Crea un oggetto della classe Document
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
                                       IsHyperlink = true,
                                       HyperlinkAddress = "www.google.com"
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

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [ITaggable](../itaggable/)
* spazio dei nomi [Aspose.Note](../../aspose.note/)
* assemblea [Aspose.Note](../../)


