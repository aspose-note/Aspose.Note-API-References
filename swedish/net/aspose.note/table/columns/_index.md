---
title: Columns
second_title: Aspose.Note för .NET API-referens
description: Hämtar tabellens kolumner.
type: docs
weight: 20
url: /sv/net/aspose.note/table/columns/
---
## Table.Columns property

Hämtar tabellens kolumner.

```csharp
public IList<TableColumn> Columns { get; }
```

### Exempel

Visar hur man ställer in en bakgrundsfärg för en cell.

```csharp
// Skapa ett objekt av klassen Document
Document doc = new Document();

// Initiera TableCell-klassobjekt och ställ in textinnehåll
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
cell11.BackgroundColor = Color.Coral;

// Initiera TableRow-klassobjekt
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

// Initiera Sidklassobjekt
Page page = new Page(doc);
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

Visar hur man lägger till ny tabell med tagg.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Tags();

// Skapa ett objekt av klassen Document
Document doc = new Document();

// Initiera Sidklassobjekt
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initiera TableRow-klassobjekt
TableRow row = new TableRow(doc);

// Initiera TableCell-klassobjekt
TableCell cell = new TableCell(doc);

// Infoga cellinnehåll
cell.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Single cell."));

// Lägg till cell till radnod
row.AppendChildLast(cell);

// Initiera tabellnod
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70 } }
              };

// Infoga radnod i tabellen
table.AppendChildLast(row);

// Lägg till tagg till denna tabellnod
table.Tags.Add(NoteTag.CreateQuestionMark());

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// Lägg till tabellnod
outlineElem.AppendChildLast(table);

// Lägg till konturelement
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// Spara OneNote-dokument
dataDir = dataDir + "AddTableNodeWithTag_out.one";
doc.Save(dataDir);
```

Visar hur man skapar en tabell med en låst kolumn.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Tables();

// Skapa ett objekt av klassen Document
Document doc = new Document();

// Initiera Sidklassobjekt
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initiera TableRow-klassobjekt
TableRow row1 = new TableRow(doc);

// Initiera TableCell-klassobjekt och ställ in textinnehåll
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
row1.AppendChildLast(cell11);

// Initiera TableRow-klassobjekt
TableRow row2 = new TableRow(doc);

// Initiera TableCell-klassobjekt och ställ in textinnehåll
TableCell cell21 = new TableCell(doc);
cell21.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Long   text    with    several   words and    spaces."));
row2.AppendChildLast(cell21);

// Initiera Table-klassobjekt
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70, LockedWidth = true } }
              };

// Lägg till rader
table.AppendChildLast(row1);
table.AppendChildLast(row2);

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// Lägg till tabellnod
outlineElem.AppendChildLast(table);

// Lägg till nod för dispositionselement
outline.AppendChildLast(outlineElem);

// Lägg till dispositionsnod
page.AppendChildLast(outline);

// Lägg till sidnod
doc.AppendChildLast(page);
dataDir = dataDir + "CreateTableWithLockedColumns_out.one";
doc.Save(dataDir);
```

Visar hur man skapar en ny tabell.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Tables();

// Skapa ett objekt av klassen Document
Document doc = new Document();

// Initiera Sidklassobjekt
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initiera TableRow-klassobjekt
TableRow row1 = new TableRow(doc);

// Initiera TableCell-klassobjekt
TableCell cell11 = new TableCell(doc);
TableCell cell12 = new TableCell(doc);
TableCell cell13 = new TableCell(doc);

// Lägg till dispositionselement i tabellcellen
cell11.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.1"));
cell12.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.2"));
cell13.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.3"));

// Tabell celler till rader
row1.AppendChildLast(cell11);
row1.AppendChildLast(cell12);
row1.AppendChildLast(cell13);

// Initiera TableRow-klassobjekt
TableRow row2 = new TableRow(doc);

// initiera TableCell-klassobjekt
TableCell cell21 = new TableCell(doc);
TableCell cell22 = new TableCell(doc);
TableCell cell23 = new TableCell(doc);

// Lägg till dispositionselement i tabellcellen
cell21.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.1"));
cell22.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.2"));
cell23.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.3"));

// Lägg till tabellceller till rader
row2.AppendChildLast(cell21);
row2.AppendChildLast(cell22);
row2.AppendChildLast(cell23);

// Initiera Table-klassobjekt och ange kolumnbredder
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 200 }, new TableColumn { Width = 200 }, new TableColumn { Width = 200 } }
              };

// Lägg till tabellrader i tabellen
table.AppendChildLast(row1);
table.AppendChildLast(row2);

// Initiera Outline-objekt
Outline outline = new Outline(doc);

// Initiera OutlineElement-objekt
OutlineElement outlineElem = new OutlineElement(doc);

// Lägg till tabell till konturelementnoden
outlineElem.AppendChildLast(table);

// Lägg till dispositionselement till disposition
outline.AppendChildLast(outlineElem);

// Lägg till disposition till sidnoden
page.AppendChildLast(outline);

// Lägg till sida till dokumentnoden
doc.AppendChildLast(page);
dataDir = dataDir + "InsertTable_out.one";
doc.Save(dataDir);
```

### Se även

* class [TableColumn](../../tablecolumn)
* class [Table](../../table)
* namnutrymme [Aspose.Note](../../table)
* hopsättning [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
