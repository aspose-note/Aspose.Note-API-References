---
title: TableColumn.LockedWidth
second_title: Référence de l'API Aspose.Note pour .NET
description: TableColumn propriété. Obtient ou définit une valeur indiquant si une colonne de tableau a une largeur verrouillée et ne se redimensionne pas automatiquement pour sadapter au contenu du tableau. Par défaut la largeur de colonne nest pas verrouillée.
type: docs
weight: 20
url: /fr/net/aspose.note/tablecolumn/lockedwidth/
---
## TableColumn.LockedWidth property

Obtient ou définit une valeur indiquant si une colonne de tableau a une largeur verrouillée et ne se redimensionne pas automatiquement pour s'adapter au contenu du tableau. Par défaut, la largeur de colonne n'est pas verrouillée.

```csharp
public bool LockedWidth { get; set; }
```

### Exemples

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

### Voir également

* class [TableColumn](../)
* espace de noms [Aspose.Note](../../tablecolumn/)
* Assemblée [Aspose.Note](../../../)


