---
title: TableColumn.LockedWidth
second_title: Aspose.Note für .NET-API-Referenz
description: TableColumn eigendom. Ruft einen Wert ab oder legt einen Wert fest der angibt ob eine Tabellenspalte eine gesperrte Breite hat und die Größe nicht automatisch an den Tabelleninhalt angepasst wird. Standardmäßig ist die Spaltenbreite nicht gesperrt.
type: docs
weight: 20
url: /de/net/aspose.note/tablecolumn/lockedwidth/
---
## TableColumn.LockedWidth property

Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob eine Tabellenspalte eine gesperrte Breite hat und die Größe nicht automatisch an den Tabelleninhalt angepasst wird. Standardmäßig ist die Spaltenbreite nicht gesperrt.

```csharp
public bool LockedWidth { get; set; }
```

### Beispiele

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

### Siehe auch

* class [TableColumn](../)
* namensraum [Aspose.Note](../../tablecolumn/)
* Montage [Aspose.Note](../../../)


