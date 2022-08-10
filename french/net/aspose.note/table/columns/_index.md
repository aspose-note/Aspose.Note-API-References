---
title: Columns
second_title: Référence de l'API Aspose.Note pour .NET
description: Obtient les colonnes de la table.
type: docs
weight: 20
url: /fr/net/aspose.note/table/columns/
---
## Table.Columns property

Obtient les colonnes de la table.

```csharp
public IList<TableColumn> Columns { get; }
```

### Exemples

Montre comment définir une couleur d'arrière-plan pour une cellule.

```csharp
// Crée un objet de la classe Document
Document doc = new Document();

// Initialise l'objet de classe TableCell et définit le contenu du texte
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
cell11.BackgroundColor = Color.Coral;

// Initialise l'objet de classe TableRow
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

// Initialise l'objet de la classe Page
Page page = new Page(doc);
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

Montre comment ajouter une nouvelle table avec une balise.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Tags();

// Crée un objet de la classe Document
Document doc = new Document();

// Initialise l'objet de la classe Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialise l'objet de classe TableRow
TableRow row = new TableRow(doc);

// Initialise l'objet de classe TableCell
TableCell cell = new TableCell(doc);

// Insérer le contenu de la cellule
cell.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Single cell."));

// Ajouter une cellule au nœud de ligne
row.AppendChildLast(cell);

// Initialise le nœud de la table
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70 } }
              };

// Insérer un nœud de ligne dans le tableau
table.AppendChildLast(row);

// Ajouter une balise à ce nœud de table
table.Tags.Add(NoteTag.CreateQuestionMark());

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// Ajouter un nœud de table
outlineElem.AppendChildLast(table);

// Ajout d'éléments de contour
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// Enregistrer le document OneNote
dataDir = dataDir + "AddTableNodeWithTag_out.one";
doc.Save(dataDir);
```

Montre comment créer une table avec une colonne verrouillée.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Tables();

// Crée un objet de la classe Document
Document doc = new Document();

// Initialise l'objet de la classe Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialise l'objet de classe TableRow
TableRow row1 = new TableRow(doc);

// Initialise l'objet de classe TableCell et définit le contenu du texte
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
row1.AppendChildLast(cell11);

// Initialise l'objet de classe TableRow
TableRow row2 = new TableRow(doc);

// Initialise l'objet de classe TableCell et définit le contenu du texte
TableCell cell21 = new TableCell(doc);
cell21.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Long   text    with    several   words and    spaces."));
row2.AppendChildLast(cell21);

// Initialise l'objet de classe Table
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70, LockedWidth = true } }
              };

// Ajouter des lignes
table.AppendChildLast(row1);
table.AppendChildLast(row2);

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// Ajouter un nœud de table
outlineElem.AppendChildLast(table);

// Ajoute un nœud d'élément de contour
outline.AppendChildLast(outlineElem);

// Ajoute un nœud de contour
page.AppendChildLast(outline);

// Ajouter un nœud de page
doc.AppendChildLast(page);
dataDir = dataDir + "CreateTableWithLockedColumns_out.one";
doc.Save(dataDir);
```

Montre comment créer une nouvelle table.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Tables();

// Crée un objet de la classe Document
Document doc = new Document();

// Initialise l'objet de la classe Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialise l'objet de classe TableRow
TableRow row1 = new TableRow(doc);

// Initialise les objets de la classe TableCell
TableCell cell11 = new TableCell(doc);
TableCell cell12 = new TableCell(doc);
TableCell cell13 = new TableCell(doc);

// Ajoute des éléments de contour dans la cellule du tableau
cell11.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.1"));
cell12.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.2"));
cell13.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.3"));

// Cellules du tableau en lignes
row1.AppendChildLast(cell11);
row1.AppendChildLast(cell12);
row1.AppendChildLast(cell13);

// Initialise l'objet de classe TableRow
TableRow row2 = new TableRow(doc);

// initialise les objets de la classe TableCell
TableCell cell21 = new TableCell(doc);
TableCell cell22 = new TableCell(doc);
TableCell cell23 = new TableCell(doc);

// Ajoute des éléments de contour dans la cellule du tableau
cell21.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.1"));
cell22.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.2"));
cell23.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.3"));

// Ajoute les cellules du tableau aux lignes
row2.AppendChildLast(cell21);
row2.AppendChildLast(cell22);
row2.AppendChildLast(cell23);

// Initialise l'objet de classe Table et définit les largeurs de colonne
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 200 }, new TableColumn { Width = 200 }, new TableColumn { Width = 200 } }
              };

// Ajoute les lignes du tableau au tableau
table.AppendChildLast(row1);
table.AppendChildLast(row2);

// Initialise l'objet Outline
Outline outline = new Outline(doc);

// Initialise l'objet OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Ajouter un tableau au nœud de l'élément de plan
outlineElem.AppendChildLast(table);

// Ajoute un élément de contour au contour
outline.AppendChildLast(outlineElem);

// Ajoute le contour au nœud de la page
page.AppendChildLast(outline);

// Ajouter une page au nœud du document
doc.AppendChildLast(page);
dataDir = dataDir + "InsertTable_out.one";
doc.Save(dataDir);
```

### Voir également

* class [TableColumn](../../tablecolumn)
* class [Table](../../table)
* espace de noms [Aspose.Note](../../table)
* Assemblée [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
