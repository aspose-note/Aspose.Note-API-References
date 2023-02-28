---
title: Table.IsBordersVisible
second_title: Aspose.Note voor .NET API-referentie
description: Table eigendom. Haalt of stelt een waarde in die aangeeft of de tabelrand zichtbaar is.
type: docs
weight: 30
url: /nl/net/aspose.note/table/isbordersvisible/
---
## Table.IsBordersVisible property

Haalt of stelt een waarde in die aangeeft of de tabelrand zichtbaar is.

```csharp
public bool IsBordersVisible { get; set; }
```

### Voorbeelden

Laat zien hoe u een achtergrondkleur voor een cel instelt.

```csharp
// Maak een object van de klasse Document
Document doc = new Document();

// Initialiseer het klasseobject TableCell en stel tekstinhoud in
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
cell11.BackgroundColor = Color.Coral;

// Initialiseer het klasseobject TableRow
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

// Initialiseer het paginaklasse-object
Page page = new Page(doc);
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

Laat zien hoe een nieuwe tabel met tag kan worden toegevoegd.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Tags();

// Maak een object van de klasse Document
Document doc = new Document();

// Initialiseer het paginaklasse-object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialiseer het klasseobject TableRow
TableRow row = new TableRow(doc);

// Initialiseer het klasseobject TableCell
TableCell cell = new TableCell(doc);

// Celinhoud invoegen
cell.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Single cell."));

// Voeg cel toe aan rijknooppunt
row.AppendChildLast(cell);

// Initialiseer tabelknooppunt
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70 } }
              };

// Voeg een rijknooppunt in de tabel in
table.AppendChildLast(row);

// Voeg een tag toe aan dit tabelknooppunt
table.Tags.Add(NoteTag.CreateQuestionMark());

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// Tabelknooppunt toevoegen
outlineElem.AppendChildLast(table);

// Voeg overzichtselementen toe
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// Sla OneNote-document op
dataDir = dataDir + "AddTableNodeWithTag_out.one";
doc.Save(dataDir);
```

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

Laat zien hoe je een nieuwe tabel maakt.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Tables();

// Maak een object van de klasse Document
Document doc = new Document();

// Initialiseer het paginaklasse-object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialiseer het klasseobject TableRow
TableRow row1 = new TableRow(doc);

// Initialiseer TableCell-klasse-objecten
TableCell cell11 = new TableCell(doc);
TableCell cell12 = new TableCell(doc);
TableCell cell13 = new TableCell(doc);

// Voeg overzichtselementen toe aan de tabelcel
cell11.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.1"));
cell12.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.2"));
cell13.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.3"));

// Tabelcellen naar rijen
row1.AppendChildLast(cell11);
row1.AppendChildLast(cell12);
row1.AppendChildLast(cell13);

// Initialiseer het klasseobject TableRow
TableRow row2 = new TableRow(doc);

// initialiseer TableCell-klasse-objecten
TableCell cell21 = new TableCell(doc);
TableCell cell22 = new TableCell(doc);
TableCell cell23 = new TableCell(doc);

// Voeg overzichtselementen toe aan de tabelcel
cell21.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.1"));
cell22.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.2"));
cell23.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.3"));

// Voeg tabelcellen toe aan rijen
row2.AppendChildLast(cell21);
row2.AppendChildLast(cell22);
row2.AppendChildLast(cell23);

// Initialiseer het tabelklasse-object en stel kolombreedten in
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 200 }, new TableColumn { Width = 200 }, new TableColumn { Width = 200 } }
              };

// Voeg tabelrijen toe aan tabel
table.AppendChildLast(row1);
table.AppendChildLast(row2);

// Initialiseer het Outline-object
Outline outline = new Outline(doc);

// Initialiseer het OutlineElement-object
OutlineElement outlineElem = new OutlineElement(doc);

// Tabel toevoegen om elementknooppunt te schetsen
outlineElem.AppendChildLast(table);

// Voeg overzichtselement toe aan overzicht
outline.AppendChildLast(outlineElem);

// Voeg overzicht toe aan paginaknooppunt
page.AppendChildLast(outline);

// Pagina toevoegen aan documentknooppunt
doc.AppendChildLast(page);
dataDir = dataDir + "InsertTable_out.one";
doc.Save(dataDir);
```

### Zie ook

* class [Table](../)
* naamruimte [Aspose.Note](../../table/)
* montage [Aspose.Note](../../../)


