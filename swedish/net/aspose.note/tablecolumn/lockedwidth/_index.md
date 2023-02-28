---
title: TableColumn.LockedWidth
second_title: Aspose.Note för .NET API-referens
description: TableColumn fast egendom. Hämtar eller ställer in ett värde som anger om en tabellkolumn har låst bredd och inte ändrar storlek automatiskt för att passa tabellinnehåll. Som standard är kolumnbredden inte låst.
type: docs
weight: 20
url: /sv/net/aspose.note/tablecolumn/lockedwidth/
---
## TableColumn.LockedWidth property

Hämtar eller ställer in ett värde som anger om en tabellkolumn har låst bredd och inte ändrar storlek automatiskt för att passa tabellinnehåll. Som standard är kolumnbredden inte låst.

```csharp
public bool LockedWidth { get; set; }
```

### Exempel

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

### Se även

* class [TableColumn](../)
* namnutrymme [Aspose.Note](../../tablecolumn/)
* hopsättning [Aspose.Note](../../../)


