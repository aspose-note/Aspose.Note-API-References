---
title: TableColumn.LockedWidth
second_title: Aspose.Note per .NET API Reference
description: TableColumn proprietà. Ottiene o imposta un valore che indica se una colonna della tabella ha una larghezza bloccata e non viene ridimensionata automaticamente per adattarsi al contenuto della tabella. Per impostazione predefinita la larghezza della colonna non è bloccata.
type: docs
weight: 20
url: /it/net/aspose.note/tablecolumn/lockedwidth/
---
## TableColumn.LockedWidth property

Ottiene o imposta un valore che indica se una colonna della tabella ha una larghezza bloccata e non viene ridimensionata automaticamente per adattarsi al contenuto della tabella. Per impostazione predefinita, la larghezza della colonna non è bloccata.

```csharp
public bool LockedWidth { get; set; }
```

### Esempi

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

### Guarda anche

* class [TableColumn](../)
* spazio dei nomi [Aspose.Note](../../tablecolumn/)
* assemblea [Aspose.Note](../../../)


