---
title: Class TableCell
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.TableCell klas. Vertegenwoordigt een tabelcel.
type: docs
weight: 910
url: /nl/net/aspose.note/tablecell/
---
## TableCell class

Vertegenwoordigt een tabelcel.

```csharp
public sealed class TableCell : CompositeNode<IOutlineChildNode>
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [TableCell](tablecell/#constructor)() | Initialiseert een nieuw exemplaar van het`TableCell` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [BackgroundColor](../../aspose.note/tablecell/backgroundcolor/) { get; set; } | Krijgt of stelt de achtergrondkleur in. |
| [Document](../../aspose.note/node/document/) { get; } | Haalt het document van het knooppunt op. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [LastModifiedTime](../../aspose.note/tablecell/lastmodifiedtime/) { get; set; } | Haalt of stelt de laatst gewijzigde tijd in. |
| [MaxWidth](../../aspose.note/tablecell/maxwidth/) { get; } | Haalt de maximale breedte op. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Haalt het volgende knooppunt op op hetzelfde knooppuntboomniveau. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Haalt het knooppunttype op. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Haalt het bovenliggende knooppunt op. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Haalt het vorige knooppunt op hetzelfde knooppuntboomniveau. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| override [Accept](../../aspose.note/tablecell/accept/)(DocumentVisitor) | Accepteert de bezoeker van de node. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;IOutlineChildNode&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params IOutlineChildNode[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |

### Voorbeelden

Laat zien hoe tekst uit de cellen van een tabel kan worden gehaald.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Tables();

// Laad het document in Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Krijg een lijst met tabelknooppunten
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // Doorloop tabelrijen
    foreach (TableRow row in table)
    {
        // Krijg een lijst met TableCell-knooppunten
        // Doorloop tabelcellen
        foreach (TableCell cell in row)
        {
            // Tekst ophalen
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // Print tekst op het uitvoerscherm
            Console.WriteLine(text);
        }
    }
}
```

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

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* interface [IOutlineChildNode](../ioutlinechildnode/)
* naamruimte [Aspose.Note](../../aspose.note/)
* montage [Aspose.Note](../../)


