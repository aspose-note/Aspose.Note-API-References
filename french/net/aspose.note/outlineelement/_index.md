---
title: OutlineElement
second_title: Référence de l'API Aspose.Note pour .NET
description: Représente un OutlineElement.
type: docs
weight: 440
url: /fr/net/aspose.note/outlineelement/
---
## OutlineElement class

Représente un OutlineElement.

```csharp
public sealed class OutlineElement : CompositeNode<IOutlineElementChildNode>, IOutlineChildNode, 
    IOutlineElementChildNode
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [OutlineElement](outlineelement#constructor)() | Initialise une nouvelle instance du[`OutlineElement`](../outlineelement) classe. |

## Propriétés

| Nom | La description |
| --- | --- |
| [CreationTime](../../aspose.note/outlineelement/creationtime) { get; set; } | Obtient ou définit l'heure de création. |
| [Document](../../aspose.note/node/document) { get; } | Obtient le document du nœud. |
| [FirstChild](../../aspose.note/compositenode`1/firstchild) { get; } |  |
| [IndentPosition](../../aspose.note/outlineelement/indentposition) { get; set; } | Obtient ou définit la position du retrait. |
| [IsComposite](../../aspose.note/compositenode`1/iscomposite) { get; } |  |
| [LastChild](../../aspose.note/compositenode`1/lastchild) { get; } |  |
| [LastModifiedTime](../../aspose.note/outlineelement/lastmodifiedtime) { get; set; } | Obtient ou définit l'heure de la dernière modification. |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | Obtient le nœud suivant au même niveau d'arborescence de nœuds. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | Obtient le type de nœud. |
| [NumberList](../../aspose.note/outlineelement/numberlist) { get; set; } | Obtient ou définit le style de l'en-tête de la liste numérotée. |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | Obtient le nœud parent. |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | Obtient le nœud précédent au même niveau d'arborescence de nœuds. |

## Méthodes

| Nom | La description |
| --- | --- |
| override [Accept](../../aspose.note/outlineelement/accept)(DocumentVisitor) | Accepte le visiteur du nœud. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildfirst)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildlast)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode`1/getchildnodes)() |  |
| [GetEnumerator](../../aspose.note/compositenode`1/getenumerator)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode`1/insertchild)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, IEnumerable&lt;IOutlineElementChildNode&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, params IOutlineElementChildNode[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode`1/removechild)(T1) |  |

### Exemples

Montre comment ajouter une nouvelle image avec une balise.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Tags();

// Crée un objet de la classe Document
Document doc = new Document();

// Initialise l'objet de la classe Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialise l'objet de la classe Outline
Outline outline = new Outline(doc);

// Initialise l'objet de classe OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Charger une image
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

// Insérer l'image dans le nœud du document
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// Ajoute un nœud d'élément de contour
outline.AppendChildLast(outlineElem);

// Ajoute un nœud de contour
page.AppendChildLast(outline);

// Ajouter un nœud de page
doc.AppendChildLast(page);

// Enregistrer le document OneNote
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
```

Montre comment récupérer des informations sur le formatage de la liste.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// Récupère une collection de nœuds de l'élément de contour
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// Itérer à travers chaque nœud
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // Récupérer le nom de la police
        Console.WriteLine("Font Name: " + list.Font);

        // Récupère la longueur de la police
        Console.WriteLine("Font Length: " + list.Font.Length);

        // Récupère la taille de la police
        Console.WriteLine("Font Size: " + list.FontSize);

        // Récupère la couleur de la police
        Console.WriteLine("Font Color: " + list.FontColor);

        // Récupérer le format
        Console.WriteLine("Font format: " + list.Format);

        // Cochez gras
        Console.WriteLine("Is bold: " + list.IsBold);

        // Vérifier l'italique
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

Montre comment insérer une nouvelle liste avec une numérotation chinoise.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Initialiser le document OneNote
Aspose.Note.Document doc = new Aspose.Note.Document();

// Initialiser la page OneNote
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// Appliquer les paramètres de style de texte
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Les nombres dans le même plan sont automatiquement incrémentés.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

//------------------------
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

//------------------------
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

//------------------------
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// Enregistrer le document OneNote
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

Montre comment insérer de nouvelles listes à puces.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Crée un objet de la classe Document
Aspose.Note.Document doc = new Aspose.Note.Document();

// Initialise l'objet de la classe Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialise l'objet de la classe Outline
Outline outline = new Outline(doc);

// Initialise l'objet de classe TextStyle et définit les propriétés de formatage
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Initialise les objets de la classe OutlineElement et applique les puces
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// Initialise l'objet de classe RichText et applique le style de texte
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Ajout d'éléments de contour
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Ajouter un noeud Contour
page.AppendChildLast(outline);
// Ajouter un nœud de page
doc.AppendChildLast(page);

// Enregistrer le document OneNote
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

Montre comment insérer une nouvelle liste avec numérotation.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Crée un objet de la classe Document
Document doc = new Document();

// Initialise l'objet de la classe Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialise l'objet de la classe Outline
Outline outline = new Outline(doc);

// Initialise l'objet de classe TextStyle et définit les propriétés de formatage
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Initialise les objets de la classe OutlineElement et applique la numérotation
// Les nombres dans le même plan sont automatiquement incrémentés.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Ajout d'éléments de contour
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Ajouter un noeud Contour
page.AppendChildLast(outline);

// Ajouter un nœud de page
doc.AppendChildLast(page);

// Enregistrer le document OneNote
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

### Voir également

* class [CompositeNode&lt;T&gt;](../compositenode-1)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode)
* interface [IOutlineChildNode](../ioutlinechildnode)
* espace de noms [Aspose.Note](../../aspose.note)
* Assemblée [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
