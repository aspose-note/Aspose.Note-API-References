---
title: TableCell.BackgroundColor
second_title: Référence de l'API Aspose.Note pour .NET
description: TableCell propriété. Obtient ou définit la couleur darrièreplan.
type: docs
weight: 20
url: /fr/net/aspose.note/tablecell/backgroundcolor/
---
## TableCell.BackgroundColor property

Obtient ou définit la couleur d'arrière-plan.

```csharp
public Color BackgroundColor { get; set; }
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

### Voir également

* class [TableCell](../)
* espace de noms [Aspose.Note](../../tablecell/)
* Assemblée [Aspose.Note](../../../)


