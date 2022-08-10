---
title: Image
second_title: Référence de l'API Aspose.Note pour .NET
description: Représente une image.
type: docs
weight: 240
url: /fr/net/aspose.note/image/
---
## Image class

Représente une image.

```csharp
public sealed class Image : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [Image](image#constructor)() | Initialise une nouvelle instance du[`Image`](../image) classe. |
| [Image](image#constructor_4)(string, Stream) | Initialise une nouvelle instance du[`Image`](../image) classe. |
| [Image](image#constructor_5)(string, string, string) | Initialise une nouvelle instance du[`Image`](../image) classe. |

## Propriétés

| Nom | La description |
| --- | --- |
| [Alignment](../../aspose.note/image/alignment) { get; set; } | Obtient ou définit l'alignement. |
| [AlternativeTextDescription](../../aspose.note/image/alternativetextdescription) { get; set; } | Obtient ou définit un corps un texte alternatif pour l'image. |
| [AlternativeTextTitle](../../aspose.note/image/alternativetexttitle) { get; set; } | Obtient ou définit un titre de texte alternatif pour l'image. |
| [Bytes](../../aspose.note/image/bytes) { get; } | Obtient le magasin de données d'image. |
| [Document](../../aspose.note/node/document) { get; } | Obtient le document du nœud. |
| [FileName](../../aspose.note/image/filename) { get; } | Récupère le nom du fichier. |
| [FilePath](../../aspose.note/image/filepath) { get; } | Obtient le chemin d'accès au fichier image. |
| [Format](../../aspose.note/image/format) { get; } | Obtient le format de l'image. |
| [Height](../../aspose.note/image/height) { get; set; } | Obtient ou définit la hauteur. Il s'agit de la hauteur réelle de l'image dans le document MS OneNote. |
| [HorizontalOffset](../../aspose.note/image/horizontaloffset) { get; set; } | Obtient ou définit le décalage horizontal. |
| [HyperlinkUrl](../../aspose.note/image/hyperlinkurl) { get; set; } | Obtient ou définit le lien hypertexte associé à l'image. |
| [IsBackground](../../aspose.note/image/isbackground) { get; set; } | Obtient si l'image est une image d'arrière-plan. |
| virtual [IsComposite](../../aspose.note/node/iscomposite) { get; } | Obtient une valeur indiquant si ce nœud est composite. Si vrai, le nœud peut avoir des nœuds enfants. |
| [LastModifiedTime](../../aspose.note/image/lastmodifiedtime) { get; set; } | Obtient ou définit l'heure de la dernière modification. |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | Obtient le nœud suivant au même niveau d'arborescence de nœuds. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | Obtient le type de nœud. |
| [OriginalHeight](../../aspose.note/image/originalheight) { get; } | Obtient la hauteur d'origine. Il s'agit de la largeur d'origine de l'image, avant redimensionnement. |
| [OriginalWidth](../../aspose.note/image/originalwidth) { get; } | Obtient la largeur d'origine. Il s'agit de la largeur d'origine de l'image, avant redimensionnement. |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | Obtient le nœud parent. |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | Obtient le nœud précédent au même niveau d'arborescence de nœuds. |
| [Tags](../../aspose.note/image/tags) { get; } | Obtient la liste de toutes les balises d'un paragraphe. |
| [VerticalOffset](../../aspose.note/image/verticaloffset) { get; set; } | Obtient ou définit le décalage vertical. |
| [Width](../../aspose.note/image/width) { get; set; } | Obtient ou définit la largeur. Il s'agit de la largeur réelle de l'image dans le document MS OneNote. |

## Méthodes

| Nom | La description |
| --- | --- |
| override [Accept](../../aspose.note/image/accept)(DocumentVisitor) | Accepte le visiteur du nœud. |

### Exemples

Montre comment lier un lien hypertexte à une image.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://image.com" } ;

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

Montre comment définir la description textuelle d'une image.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Images();

var document = new Document();
var page = new Page(document);
var image = new Image(document, dataDir + "image.jpg")
            {
                AlternativeTextTitle = "This is an image's title!",
                AlternativeTextDescription = "And this is an image's description!"
            };
page.AppendChildLast(image);
document.AppendChildLast(page);

dataDir = dataDir + "ImageAlternativeText_out.one";
document.Save(dataDir);
```

Montre comment obtenir une image à partir d'un document.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Images();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Récupère tous les nœuds Image
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Enregistre les octets de l'image dans un fichier
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

Montre comment obtenir les méta-informations de l'image.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Images();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Récupère tous les nœuds Image
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

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

Montre comment ajouter une image d'un fichier à un document avec des propriétés définies par l'utilisateur.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Images();

// Charge le document à partir du flux.
Document doc = new Document(dataDir + "Aspose.one");

// Récupère la première page du document.
Aspose.Note.Page page = doc.FirstChild;

// Charge une image à partir du fichier.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Modifiez la taille de l'image selon vos besoins (optionnel).
                              Width = 100,
                              Height = 100,

                              // Définit l'emplacement de l'image dans la page (optionnel).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // Définir l'alignement de l'image
                              Alignment = HorizontalAlignment.Right
                          };

// Ajoute l'image à la page.
page.AppendChildLast(image);
```

Montre comment ajouter une image du flux à un document.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Images();

// Crée un objet de la classe Document
Document doc = new Document();

// Initialise l'objet de la classe Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // Charge la deuxième image en utilisant le nom, l'extension et le flux de l'image.
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // Définir l'alignement de l'image
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// Enregistrer le document OneNote
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

Montre comment ajouter une image d'un fichier à un document.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Images();

// Crée un objet de la classe Document
Document doc = new Document();

// Initialise l'objet de la classe Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialise l'objet de la classe Outline et définit les propriétés de décalage
Outline outline = new Outline(doc);

// Initialise l'objet de classe OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Charge une image par le chemin du fichier.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Définir l'alignement de l'image
                              Alignment = HorizontalAlignment.Right
                          };

// Ajouter une image
outlineElem.AppendChildLast(image);

// Ajout d'éléments de contour
outline.AppendChildLast(outlineElem);

// Ajouter un noeud Contour
page.AppendChildLast(outline);

// Ajouter un nœud de page
doc.AppendChildLast(page);

// Enregistrer le document OneNote
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

### Voir également

* class [Node](../node)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode)
* interface [IPageChildNode](../ipagechildnode)
* interface [ITaggable](../itaggable)
* espace de noms [Aspose.Note](../../aspose.note)
* Assemblée [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
