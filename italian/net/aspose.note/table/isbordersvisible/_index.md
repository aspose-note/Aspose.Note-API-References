---
title: Table.IsBordersVisible
second_title: Aspose.Note per .NET API Reference
description: Table proprietà. Ottiene o imposta un valore che indica se il bordo della tabella è visibile.
type: docs
weight: 30
url: /it/net/aspose.note/table/isbordersvisible/
---
## Table.IsBordersVisible property

Ottiene o imposta un valore che indica se il bordo della tabella è visibile.

```csharp
public bool IsBordersVisible { get; set; }
```

### Esempi

Mostra come impostare un colore di sfondo per una cella.

```csharp
// Crea un oggetto della classe Document
Document doc = new Document();

// Inizializza l'oggetto della classe TableCell e imposta il contenuto del testo
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
cell11.BackgroundColor = Color.Coral;

// Inizializza l'oggetto della classe TableRow
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

// Inizializza l'oggetto della classe Page
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

// Inizializza l'oggetto della classe Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inizializza l'oggetto della classe TableRow
TableRow row = new TableRow(doc);

// Inizializza l'oggetto della classe TableCell
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

// Inserisci il nodo riga nella tabella
table.AppendChildLast(row);

// Aggiungi tag a questo nodo della tabella
table.Tags.Add(NoteTag.CreateQuestionMark());

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// Aggiungi il nodo della tabella
outlineElem.AppendChildLast(table);

// Aggiungi elementi di contorno
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// Salva documento OneNote
dataDir = dataDir + "AddTableNodeWithTag_out.one";
doc.Save(dataDir);
```

Mostra come creare una tabella con una colonna bloccata.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Tables();

// Crea un oggetto della classe Document
Document doc = new Document();

// Inizializza l'oggetto della classe Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inizializza l'oggetto della classe TableRow
TableRow row1 = new TableRow(doc);

// Inizializza l'oggetto della classe TableCell e imposta il contenuto del testo
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
row1.AppendChildLast(cell11);

// Inizializza l'oggetto della classe TableRow
TableRow row2 = new TableRow(doc);

// Inizializza l'oggetto della classe TableCell e imposta il contenuto del testo
TableCell cell21 = new TableCell(doc);
cell21.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Long   text    with    several   words and    spaces."));
row2.AppendChildLast(cell21);

// Inizializza l'oggetto della classe Table
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

// Aggiungi il nodo della tabella
outlineElem.AppendChildLast(table);

// Aggiungi nodo elemento contorno
outline.AppendChildLast(outlineElem);

// Aggiungi nodo di contorno
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

// Inizializza l'oggetto della classe Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inizializza l'oggetto della classe TableRow
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

// Inizializza l'oggetto della classe TableRow
TableRow row2 = new TableRow(doc);

// inizializza gli oggetti della classe TableCell
TableCell cell21 = new TableCell(doc);
TableCell cell22 = new TableCell(doc);
TableCell cell23 = new TableCell(doc);

// Aggiunge elementi di struttura nella cella della tabella
cell21.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.1"));
cell22.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.2"));
cell23.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.3"));

// Accoda le celle della tabella alle righe
row2.AppendChildLast(cell21);
row2.AppendChildLast(cell22);
row2.AppendChildLast(cell23);

// Inizializza l'oggetto della classe Table e imposta la larghezza delle colonne
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 200 }, new TableColumn { Width = 200 }, new TableColumn { Width = 200 } }
              };

// Aggiunge le righe della tabella alla tabella
table.AppendChildLast(row1);
table.AppendChildLast(row2);

// Inizializza l'oggetto Outline
Outline outline = new Outline(doc);

// Inizializza l'oggetto OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Aggiungi tabella al nodo elemento contorno
outlineElem.AppendChildLast(table);

// Aggiungi un elemento di contorno al contorno
outline.AppendChildLast(outlineElem);

// Aggiungi contorno al nodo della pagina
page.AppendChildLast(outline);

// Aggiungi pagina al nodo del documento
doc.AppendChildLast(page);
dataDir = dataDir + "InsertTable_out.one";
doc.Save(dataDir);
```

### Guarda anche

* class [Table](../)
* spazio dei nomi [Aspose.Note](../../table/)
* assemblea [Aspose.Note](../../../)


