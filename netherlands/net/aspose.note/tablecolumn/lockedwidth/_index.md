---
title: TableColumn.LockedWidth
second_title: Aspose.Note voor .NET API-referentie
description: TableColumn eigendom. Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of een tabelkolom een vergrendelde breedte heeft en niet automatisch wordt aangepast aan de inhoud van de tabel. Standaard is de kolombreedte niet vergrendeld.
type: docs
weight: 20
url: /nl/net/aspose.note/tablecolumn/lockedwidth/
---
## TableColumn.LockedWidth property

Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of een tabelkolom een vergrendelde breedte heeft en niet automatisch wordt aangepast aan de inhoud van de tabel. Standaard is de kolombreedte niet vergrendeld.

```csharp
public bool LockedWidth { get; set; }
```

### Voorbeelden

Laat zien hoe u een tabel maakt met een vergrendelde kolom.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Tables();

// Maak een object van de klasse Document
Document doc = new Document();

// Initialiseer het paginaklasse-object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialiseer het klasseobject TableRow
TableRow row1 = new TableRow(doc);

// Initialiseer het klasseobject TableCell en stel tekstinhoud in
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
row1.AppendChildLast(cell11);

// Initialiseer het klasseobject TableRow
TableRow row2 = new TableRow(doc);

// Initialiseer het klasseobject TableCell en stel tekstinhoud in
TableCell cell21 = new TableCell(doc);
cell21.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Long   text    with    several   words and    spaces."));
row2.AppendChildLast(cell21);

// Initialiseer het tabelklasse-object
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70, LockedWidth = true } }
              };

// Voeg rijen toe
table.AppendChildLast(row1);
table.AppendChildLast(row2);

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// Tabelknooppunt toevoegen
outlineElem.AppendChildLast(table);

// Voeg overzichtselementknooppunt toe
outline.AppendChildLast(outlineElem);

// Voeg overzichtsknooppunt toe
page.AppendChildLast(outline);

// Paginaknooppunt toevoegen
doc.AppendChildLast(page);
dataDir = dataDir + "CreateTableWithLockedColumns_out.one";
doc.Save(dataDir);
```

### Zie ook

* class [TableColumn](../)
* naamruimte [Aspose.Note](../../tablecolumn/)
* montage [Aspose.Note](../../../)


