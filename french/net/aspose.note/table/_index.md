---
title: Class Table
second_title: Référence de l'API Aspose.Note pour .NET
description: Aspose.Note.Table classe. Représente un tableau.
type: docs
weight: 900
url: /fr/net/aspose.note/table/
---
## Table class

Représente un tableau.

```csharp
public sealed class Table : CompositeNode<TableRow>, IOutlineElementChildNode, ITaggable
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [Table](table/#constructor)() | Initialise une nouvelle instance du`Table` classe. |

## Propriétés

| Nom | La description |
| --- | --- |
| [Columns](../../aspose.note/table/columns/) { get; } | Obtient les colonnes de la table. |
| [Document](../../aspose.note/node/document/) { get; } | Obtient le document du nœud. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IsBordersVisible](../../aspose.note/table/isbordersvisible/) { get; set; } | Obtient ou définit une valeur indiquant si la bordure du tableau est visible. |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [LastModifiedTime](../../aspose.note/table/lastmodifiedtime/) { get; set; } | Obtient ou définit l'heure de la dernière modification. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Obtient le nœud suivant au même niveau d'arborescence de nœuds. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Obtient le type de nœud. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Obtient le nœud parent. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Obtient le nœud précédent au même niveau d'arborescence de nœuds. |
| [Tags](../../aspose.note/table/tags/) { get; } | Obtient la liste de toutes les balises d'un paragraphe. |

## Méthodes

| Nom | La description |
| --- | --- |
| override [Accept](../../aspose.note/table/accept/)(DocumentVisitor) | Accepte le visiteur du nœud. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;TableRow&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params TableRow[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |

### Exemples

Montre comment obtenir du texte à partir de la ligne de chaque tableau.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Tables();

// Charge le document dans Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Récupère une liste des nœuds de la table
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // Itérer dans les lignes du tableau
    foreach (TableRow row in table)
    {
        // Récupérer le texte
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // Affiche le texte sur l'écran de sortie
        Console.WriteLine(text);
    }
}
```

Montre comment obtenir du texte à partir d'un tableau.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Tables();

// Charge le document dans Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Récupère une liste des nœuds de la table
IList<Table> nodes = document.GetChildNodes<Table>();

// Définir le nombre de tables
int tblCount = 0;

foreach (Table table in nodes)
{
    tblCount++;
    Console.WriteLine("table # " + tblCount);

    // Récupérer le texte
    string text = string.Join(Environment.NewLine, table.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

    // Affiche le texte sur l'écran de sortie
    Console.WriteLine(text);
}
```

Montre comment obtenir du texte à partir des cellules d'un tableau.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Tables();

// Charge le document dans Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Récupère une liste des nœuds de la table
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // Itérer dans les lignes du tableau
    foreach (TableRow row in table)
    {
        // Récupère la liste des nœuds TableCell
        // Itérer dans les cellules du tableau
        foreach (TableCell cell in row)
        {
            // Récupérer le texte
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // Affiche le texte sur l'écran de sortie
            Console.WriteLine(text);
        }
    }
}
```

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

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* class [TableRow](../tablerow/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [ITaggable](../itaggable/)
* espace de noms [Aspose.Note](../../aspose.note/)
* Assemblée [Aspose.Note](../../)


