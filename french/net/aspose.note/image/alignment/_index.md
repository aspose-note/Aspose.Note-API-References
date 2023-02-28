---
title: Image.Alignment
second_title: Référence de l'API Aspose.Note pour .NET
description: Image propriété. Obtient ou définit lalignement.
type: docs
weight: 20
url: /fr/net/aspose.note/image/alignment/
---
## Image.Alignment property

Obtient ou définit l'alignement.

```csharp
public HorizontalAlignment Alignment { get; set; }
```

### Exemples

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

* enum [HorizontalAlignment](../../horizontalalignment/)
* class [Image](../)
* espace de noms [Aspose.Note](../../image/)
* Assemblée [Aspose.Note](../../../)


