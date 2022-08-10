---
title: NumberList
second_title: Référence de l'API Aspose.Note pour .NET
description: Représente la liste numérotée ou à puces.
type: docs
weight: 420
url: /fr/net/aspose.note/numberlist/
---
## NumberList class

Représente la liste numérotée ou à puces.

```csharp
public class NumberList
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [NumberList](numberlist#constructor_1)(string, string, int) | Initialise une nouvelle instance du[`NumberList`](../numberlist) class. Cette instance représente une liste à puces. |
| [NumberList](numberlist#constructor)(string, NumberFormat, string, int) | Initialise une nouvelle instance du[`NumberList`](../numberlist)class. Cette instance représente une liste numérotée. |

## Propriétés

| Nom | La description |
| --- | --- |
| [Font](../../aspose.note/numberlist/font) { get; set; } | Obtient ou définit le nom de la police. |
| [FontColor](../../aspose.note/numberlist/fontcolor) { get; set; } | Obtient ou définit la couleur de la police. |
| [FontSize](../../aspose.note/numberlist/fontsize) { get; set; } | Obtient ou définit la taille de la police. |
| [Format](../../aspose.note/numberlist/format) { get; set; } | Obtient ou définit le format de l'en-tête de ligne. Pour les listes à puces, représente un symbole de puce. |
| [IsBold](../../aspose.note/numberlist/isbold) { get; set; } | Obtient ou définit une valeur indiquant si le style de texte est en gras. |
| [IsItalic](../../aspose.note/numberlist/isitalic) { get; set; } | Obtient ou définit une valeur indiquant si le style de texte est en italique. |
| [LastModifiedTime](../../aspose.note/numberlist/lastmodifiedtime) { get; set; } | Obtient ou définit l'heure de la dernière modification. |
| [NumberFormat](../../aspose.note/numberlist/numberformat) { get; set; } | Obtient ou définit le format numérique utilisé pour un groupe d'objets numérotés automatiquement. Doit être nul pour les listes à puces. |
| [Restart](../../aspose.note/numberlist/restart) { get; set; } | Obtient ou définit la valeur numérique qui remplace la valeur numérique automatique de l'élément de liste. |

## Méthodes

| Nom | La description |
| --- | --- |
| [Equals](../../aspose.note/numberlist/equals#equals)(NumberList) | Détermine si l'objet spécifié est égal à l'objet actuel. |
| override [Equals](../../aspose.note/numberlist/equals#equals_1)(object) | Détermine si l'objet spécifié est égal à l'objet actuel. |
| override [GetHashCode](../../aspose.note/numberlist/gethashcode)() | Sert de fonction de hachage pour le type. |
| [GetNumberedListHeader](../../aspose.note/numberlist/getnumberedlistheader)(int) | Obtient l'en-tête de la liste numérotée. |

### Exemples

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

* espace de noms [Aspose.Note](../../aspose.note)
* Assemblée [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
