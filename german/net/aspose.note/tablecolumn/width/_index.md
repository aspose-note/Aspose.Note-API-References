---
title: Width
second_title: Aspose.Note für .NET-API-Referenz
description: Ruft die Breite ab oder legt sie fest.
type: docs
weight: 30
url: /de/net/aspose.note/tablecolumn/width/
---
## TableColumn.Width property

Ruft die Breite ab oder legt sie fest.

```csharp
public float Width { get; set; }
```

### Beispiele

Zeigt, wie eine Hintergrundfarbe für eine Zelle festgelegt wird.

```csharp
// Erstellen Sie ein Objekt der Document-Klasse
Document doc = new Document();

// Objekt der TableCell-Klasse initialisieren und Textinhalt festlegen
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
cell11.BackgroundColor = Color.Coral;

// TableRow-Klassenobjekt initialisieren
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

// Seitenklassenobjekt initialisieren
Page page = new Page(doc);
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

Zeigt, wie man eine neue Tabelle mit Tag hinzufügt.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Tags();

// Erstellen Sie ein Objekt der Document-Klasse
Document doc = new Document();

// Seitenklassenobjekt initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// TableRow-Klassenobjekt initialisieren
TableRow row = new TableRow(doc);

// TableCell-Klassenobjekt initialisieren
TableCell cell = new TableCell(doc);

// Zellinhalt einfügen
cell.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Single cell."));

// Zelle zum Zeilenknoten hinzufügen
row.AppendChildLast(cell);

// Tabellenknoten initialisieren
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70 } }
              };

// Zeilenknoten in Tabelle einfügen
table.AppendChildLast(row);

// Tag zu diesem Tabellenknoten hinzufügen
table.Tags.Add(NoteTag.CreateQuestionMark());

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// Tabellenknoten hinzufügen
outlineElem.AppendChildLast(table);

// Gliederungselemente hinzufügen
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// OneNote-Dokument speichern
dataDir = dataDir + "AddTableNodeWithTag_out.one";
doc.Save(dataDir);
```

Zeigt, wie eine Tabelle mit einer gesperrten Spalte erstellt wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Tables();

// Erstellen Sie ein Objekt der Document-Klasse
Document doc = new Document();

// Seitenklassenobjekt initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// TableRow-Klassenobjekt initialisieren
TableRow row1 = new TableRow(doc);

// Objekt der TableCell-Klasse initialisieren und Textinhalt festlegen
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
row1.AppendChildLast(cell11);

// TableRow-Klassenobjekt initialisieren
TableRow row2 = new TableRow(doc);

// Objekt der TableCell-Klasse initialisieren und Textinhalt festlegen
TableCell cell21 = new TableCell(doc);
cell21.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Long   text    with    several   words and    spaces."));
row2.AppendChildLast(cell21);

// Tabellenklassenobjekt initialisieren
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70, LockedWidth = true } }
              };

// Zeilen hinzufügen
table.AppendChildLast(row1);
table.AppendChildLast(row2);

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// Tabellenknoten hinzufügen
outlineElem.AppendChildLast(table);

// Gliederungselementknoten hinzufügen
outline.AppendChildLast(outlineElem);

// Gliederungsknoten hinzufügen
page.AppendChildLast(outline);

// Seitenknoten hinzufügen
doc.AppendChildLast(page);
dataDir = dataDir + "CreateTableWithLockedColumns_out.one";
doc.Save(dataDir);
```

Zeigt, wie eine neue Tabelle erstellt wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Tables();

// Erstellen Sie ein Objekt der Document-Klasse
Document doc = new Document();

// Seitenklassenobjekt initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// TableRow-Klassenobjekt initialisieren
TableRow row1 = new TableRow(doc);

// Objekte der TableCell-Klasse initialisieren
TableCell cell11 = new TableCell(doc);
TableCell cell12 = new TableCell(doc);
TableCell cell13 = new TableCell(doc);

// Gliederungselemente in die Tabellenzelle einfügen
cell11.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.1"));
cell12.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.2"));
cell13.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.3"));

// Tabellenzellen zu Zeilen
row1.AppendChildLast(cell11);
row1.AppendChildLast(cell12);
row1.AppendChildLast(cell13);

// TableRow-Klassenobjekt initialisieren
TableRow row2 = new TableRow(doc);

// Objekte der TableCell-Klasse initialisieren
TableCell cell21 = new TableCell(doc);
TableCell cell22 = new TableCell(doc);
TableCell cell23 = new TableCell(doc);

// Gliederungselemente in die Tabellenzelle einfügen
cell21.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.1"));
cell22.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.2"));
cell23.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.3"));

// Tabellenzellen an Zeilen anhängen
row2.AppendChildLast(cell21);
row2.AppendChildLast(cell22);
row2.AppendChildLast(cell23);

// Tabellenklassenobjekt initialisieren und Spaltenbreiten festlegen
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 200 }, new TableColumn { Width = 200 }, new TableColumn { Width = 200 } }
              };

// Tabellenzeilen an Tabelle anhängen
table.AppendChildLast(row1);
table.AppendChildLast(row2);

// Outline-Objekt initialisieren
Outline outline = new Outline(doc);

// OutlineElement-Objekt initialisieren
OutlineElement outlineElem = new OutlineElement(doc);

// Tabelle zum Gliederungselementknoten hinzufügen
outlineElem.AppendChildLast(table);

// Gliederungselement zur Gliederung hinzufügen
outline.AppendChildLast(outlineElem);

// Gliederung zum Seitenknoten hinzufügen
page.AppendChildLast(outline);

// Seite zum Dokumentknoten hinzufügen
doc.AppendChildLast(page);
dataDir = dataDir + "InsertTable_out.one";
doc.Save(dataDir);
```

### Siehe auch

* class [TableColumn](../../tablecolumn)
* namensraum [Aspose.Note](../../tablecolumn)
* Montage [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
