---
title: TableRow
second_title: Aspose.Note per .NET API Reference
description: Rappresenta una riga di tabella.
type: docs
weight: 900
url: /it/net/aspose.note/tablerow/
---
## TableRow class

Rappresenta una riga di tabella.

```csharp
public sealed class TableRow : CompositeNode<TableCell>
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [TableRow](tablerow#constructor)() | Inizializza una nuova istanza di[`TableRow`](../tablerow) classe. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Document](../../aspose.note/node/document) { get; } | Ottiene il documento del nodo. |
| [FirstChild](../../aspose.note/compositenode`1/firstchild) { get; } |  |
| [IsComposite](../../aspose.note/compositenode`1/iscomposite) { get; } |  |
| [LastChild](../../aspose.note/compositenode`1/lastchild) { get; } |  |
| [LastModifiedTime](../../aspose.note/tablerow/lastmodifiedtime) { get; set; } | Ottiene o imposta l'ultima ora modificata. |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | Ottiene il nodo successivo allo stesso livello di albero dei nodi. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | Ottiene il tipo di nodo. |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | Ottiene il nodo padre. |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | Ottiene il nodo precedente allo stesso livello di albero dei nodi. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Accept](../../aspose.note/tablerow/accept)(DocumentVisitor) | Accetta il visitatore del nodo. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildfirst)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildlast)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode`1/getchildnodes)() |  |
| [GetEnumerator](../../aspose.note/compositenode`1/getenumerator)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode`1/insertchild)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, IEnumerable&lt;TableCell&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, params TableCell[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode`1/removechild)(T1) |  |

### Esempi

Mostra come ottenere testo da ogni riga di tabella.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Tables();

// Carica il documento in Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Ottieni un elenco di nodi della tabella
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // Scorri le righe della tabella
    foreach (TableRow row in table)
    {
        // Recupera il testo
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // Stampa il testo sulla schermata di output
        Console.WriteLine(text);
    }
}
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
    // Scorri le righe della tabella
    foreach (TableRow row in table)
    {
        // Ottieni l'elenco dei nodi TableCell
        // Scorri le celle della tabella
        foreach (TableCell cell in row)
        {
            // Recupera il testo
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // Stampa il testo sulla schermata di output
            Console.WriteLine(text);
        }
    }
}
```

Mostra come impostare un colore di sfondo per una cella.

```csharp
// Crea un oggetto della classe Document
Document doc = new Document();

// Inizializza l'oggetto classe TableCell e imposta il contenuto del testo
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
cell11.BackgroundColor = Color.Coral;

// Inizializza l'oggetto classe TableRow
TableRow row = new TableRow(doc);
row.AppendChildLast(cell11);

Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn() { Width = 200 } }
              };
table.AppendChildLast(row);

OutlineElement oe = new OutlineElement(doc);
oe.AppendChildLast(table);

Outline o = new Outline(doc);
o.AppendChildLast(oe);

// Inizializza l'oggetto della classe Pagina
Page page = new Page(doc);
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

Mostra come aggiungere una nuova tabella con tag.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Tags();

// Crea un oggetto della classe Document
Document doc = new Document();

// Inizializza l'oggetto della classe Pagina
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inizializza l'oggetto classe TableRow
TableRow row = new TableRow(doc);

// Inizializza l'oggetto classe TableCell
TableCell cell = new TableCell(doc);

// Inserisci il contenuto della cella
cell.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Single cell."));

// Aggiungi cella al nodo riga
row.AppendChildLast(cell);

// Inizializza il nodo della tabella
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70 } }
              };

// Inserisce il nodo riga nella tabella
table.AppendChildLast(row);

// Aggiungi tag a questo nodo della tabella
table.Tags.Add(NoteTag.CreateQuestionMark());

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// Aggiungi nodo tabella
outlineElem.AppendChildLast(table);

// Aggiungi elementi di contorno
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// Salva il documento di OneNote
dataDir = dataDir + "AddTableNodeWithTag_out.one";
doc.Save(dataDir);
```

Mostra come creare una tabella con una colonna bloccata.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Tables();

// Crea un oggetto della classe Document
Document doc = new Document();

// Inizializza l'oggetto della classe Pagina
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inizializza l'oggetto classe TableRow
TableRow row1 = new TableRow(doc);

// Inizializza l'oggetto classe TableCell e imposta il contenuto del testo
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
row1.AppendChildLast(cell11);

// Inizializza l'oggetto classe TableRow
TableRow row2 = new TableRow(doc);

// Inizializza l'oggetto classe TableCell e imposta il contenuto del testo
TableCell cell21 = new TableCell(doc);
cell21.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Long   text    with    several   words and    spaces."));
row2.AppendChildLast(cell21);

// Inizializza l'oggetto classe Table
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70, LockedWidth = true } }
              };

// Aggiungi righe
table.AppendChildLast(row1);
table.AppendChildLast(row2);

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// Aggiungi nodo tabella
outlineElem.AppendChildLast(table);

// Aggiunge il nodo dell'elemento struttura
outline.AppendChildLast(outlineElem);

// Aggiungi nodo struttura
page.AppendChildLast(outline);

// Aggiungi il nodo della pagina
doc.AppendChildLast(page);
dataDir = dataDir + "CreateTableWithLockedColumns_out.one";
doc.Save(dataDir);
```

Mostra come creare una nuova tabella.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Tables();

// Crea un oggetto della classe Document
Document doc = new Document();

// Inizializza l'oggetto della classe Pagina
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inizializza l'oggetto classe TableRow
TableRow row1 = new TableRow(doc);

// Inizializza gli oggetti della classe TableCell
TableCell cell11 = new TableCell(doc);
TableCell cell12 = new TableCell(doc);
TableCell cell13 = new TableCell(doc);

// Aggiunge elementi di struttura nella cella della tabella
cell11.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.1"));
cell12.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.2"));
cell13.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.3"));

// Da celle di tabella a righe
row1.AppendChildLast(cell11);
row1.AppendChildLast(cell12);
row1.AppendChildLast(cell13);

// Inizializza l'oggetto classe TableRow
TableRow row2 = new TableRow(doc);

// inizializza gli oggetti della classe TableCell
TableCell cell21 = new TableCell(doc);
TableCell cell22 = new TableCell(doc);
TableCell cell23 = new TableCell(doc);

// Aggiunge elementi di struttura nella cella della tabella
cell21.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.1"));
cell22.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.2"));
cell23.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.3"));

// Aggiunge le celle della tabella alle righe
row2.AppendChildLast(cell21);
row2.AppendChildLast(cell22);
row2.AppendChildLast(cell23);

// Inizializza l'oggetto classe Table e imposta la larghezza delle colonne
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 200 }, new TableColumn { Width = 200 }, new TableColumn { Width = 200 } }
              };

// Aggiunge le righe della tabella alla tabella
table.AppendChildLast(row1);
table.AppendChildLast(row2);

// Inizializza l'oggetto Struttura
Outline outline = new Outline(doc);

// Inizializza l'oggetto OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Aggiunge una tabella al nodo dell'elemento struttura
outlineElem.AppendChildLast(table);

// Aggiungi un elemento di contorno al contorno
outline.AppendChildLast(outlineElem);

// Aggiungi struttura al nodo della pagina
page.AppendChildLast(outline);

// Aggiungi la pagina al nodo del documento
doc.AppendChildLast(page);
dataDir = dataDir + "InsertTable_out.one";
doc.Save(dataDir);
```

### Guarda anche

* class [CompositeNode&lt;T&gt;](../compositenode-1)
* class [TableCell](../tablecell)
* spazio dei nomi [Aspose.Note](../../aspose.note)
* assemblea [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
