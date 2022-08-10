---
title: NumberList
second_title: Aspose.Note per .NET API Reference
description: Rappresenta lelenco numerato o puntato.
type: docs
weight: 420
url: /it/net/aspose.note/numberlist/
---
## NumberList class

Rappresenta l'elenco numerato o puntato.

```csharp
public class NumberList
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [NumberList](numberlist#constructor_1)(string, string, int) | Inizializza una nuova istanza di[`NumberList`](../numberlist) class. Questa istanza rappresenta un elenco puntato. |
| [NumberList](numberlist#constructor)(string, NumberFormat, string, int) | Inizializza una nuova istanza di[`NumberList`](../numberlist)class. Questa istanza rappresenta un elenco numerato. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Font](../../aspose.note/numberlist/font) { get; set; } | Ottiene o imposta il nome del font. |
| [FontColor](../../aspose.note/numberlist/fontcolor) { get; set; } | Ottiene o imposta il colore del carattere. |
| [FontSize](../../aspose.note/numberlist/fontsize) { get; set; } | Ottiene o imposta la dimensione del carattere. |
| [Format](../../aspose.note/numberlist/format) { get; set; } | Ottiene o imposta il formato dell'intestazione della riga. Per gli elenchi puntati rappresenta un simbolo di punto elenco. |
| [IsBold](../../aspose.note/numberlist/isbold) { get; set; } | Ottiene o imposta un valore che indica se lo stile del testo è grassetto. |
| [IsItalic](../../aspose.note/numberlist/isitalic) { get; set; } | Ottiene o imposta un valore che indica se lo stile del testo è corsivo. |
| [LastModifiedTime](../../aspose.note/numberlist/lastmodifiedtime) { get; set; } | Ottiene o imposta l'ultima ora modificata. |
| [NumberFormat](../../aspose.note/numberlist/numberformat) { get; set; } | Ottiene o imposta il formato numerico utilizzato per un gruppo di oggetti numerati automaticamente. Dovrebbe essere nullo per gli elenchi puntati. |
| [Restart](../../aspose.note/numberlist/restart) { get; set; } | Ottiene o imposta il valore numerico che sostituisce il valore numerico automatico dell'elemento dell'elenco. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Equals](../../aspose.note/numberlist/equals#equals)(NumberList) | Determina se l'oggetto specificato è uguale all'oggetto corrente. |
| override [Equals](../../aspose.note/numberlist/equals#equals_1)(object) | Determina se l'oggetto specificato è uguale all'oggetto corrente. |
| override [GetHashCode](../../aspose.note/numberlist/gethashcode)() | Serve come funzione hash per il tipo. |
| [GetNumberedListHeader](../../aspose.note/numberlist/getnumberedlistheader)(int) | Ottiene l'intestazione dell'elenco numerato. |

### Esempi

Mostra come recuperare informazioni sulla formattazione dell'elenco.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// Recupera i nodi di una raccolta dell'elemento struttura
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// Scorri ogni nodo
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // Recupera il nome del carattere
        Console.WriteLine("Font Name: " + list.Font);

        // Recupera la lunghezza del carattere
        Console.WriteLine("Font Length: " + list.Font.Length);

        // Recupera la dimensione del carattere
        Console.WriteLine("Font Size: " + list.FontSize);

        // Recupera il colore del carattere
        Console.WriteLine("Font Color: " + list.FontColor);

        // Recupera il formato
        Console.WriteLine("Font format: " + list.Format);

        // Spunta il grassetto
        Console.WriteLine("Is bold: " + list.IsBold);

        // Controlla il corsivo
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
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

//---------------------------
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

//---------------------------
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

//---------------------------
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// Salva il documento di OneNote
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

Mostra come inserire una nuova lista con numerazione.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Crea un oggetto della classe Document
Document doc = new Document();

// Inizializza l'oggetto della classe Pagina
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inizializza l'oggetto classe Outline
Outline outline = new Outline(doc);

// Inizializza l'oggetto classe TextStyle e imposta le proprietà di formattazione
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

//Aggiungi nodo Struttura
page.AppendChildLast(outline);

// Aggiungi il nodo Pagina
doc.AppendChildLast(page);

// Salva il documento di OneNote
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

### Guarda anche

* spazio dei nomi [Aspose.Note](../../aspose.note)
* assemblea [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
