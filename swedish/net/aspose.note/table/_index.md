---
title: Class Table
second_title: Aspose.Note för .NET API-referens
description: Aspose.Note.Table klass. Representerar en tabell.
type: docs
weight: 900
url: /sv/net/aspose.note/table/
---
## Table class

Representerar en tabell.

```csharp
public sealed class Table : CompositeNode<TableRow>, IOutlineElementChildNode, ITaggable
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [Table](table/#constructor)() | Initierar en ny instans av`Table` class. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Columns](../../aspose.note/table/columns/) { get; } | Hämtar tabellens kolumner. |
| [Document](../../aspose.note/node/document/) { get; } | Hämtar dokumentet för noden. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IsBordersVisible](../../aspose.note/table/isbordersvisible/) { get; set; } | Hämtar eller ställer in ett värde som anger om tabellkanten är synlig. |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [LastModifiedTime](../../aspose.note/table/lastmodifiedtime/) { get; set; } | Hämtar eller ställer in den senast ändrade tiden. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Hämtar nästa nod på samma nodträdsnivå. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Hämtar nodtypen. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Hämtar den överordnade noden. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Hämtar föregående nod på samma nodträdsnivå. |
| [Tags](../../aspose.note/table/tags/) { get; } | Hämtar listan över alla taggar i ett stycke. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| override [Accept](../../aspose.note/table/accept/)(DocumentVisitor) | Accepterar besökaren av noden. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;TableRow&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params TableRow[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |

### Exempel

Visar hur man hämtar text från varje tabells rad.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Tables();

// Ladda dokumentet i Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Få en lista över tabellnoder
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // Iterera genom tabellrader
    foreach (TableRow row in table)
    {
        // Hämta text
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // Skriv ut text på utdataskärmen
        Console.WriteLine(text);
    }
}
```

Visar hur man hämtar text från en tabell.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Tables();

// Ladda dokumentet i Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Få en lista över tabellnoder
IList<Table> nodes = document.GetChildNodes<Table>();

// Ange tabellräkning
int tblCount = 0;

foreach (Table table in nodes)
{
    tblCount++;
    Console.WriteLine("table # " + tblCount);

    // Hämta text
    string text = string.Join(Environment.NewLine, table.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

    // Skriv ut text på utdataskärmen
    Console.WriteLine(text);
}
```

Visar hur man hämtar text från en tabells celler.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Tables();

// Ladda dokumentet i Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Få en lista över tabellnoder
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // Iterera genom tabellrader
    foreach (TableRow row in table)
    {
        // Få lista över TableCell-noder
        // Iterera genom tabellceller
        foreach (TableCell cell in row)
        {
            // Hämta text
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // Skriv ut text på utdataskärmen
            Console.WriteLine(text);
        }
    }
}
```

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

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* class [TableRow](../tablerow/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [ITaggable](../itaggable/)
* namnutrymme [Aspose.Note](../../aspose.note/)
* hopsättning [Aspose.Note](../../)


