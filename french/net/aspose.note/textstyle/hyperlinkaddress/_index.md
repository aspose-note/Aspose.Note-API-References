---
title: TextStyle.HyperlinkAddress
second_title: Référence de l'API Aspose.Note pour .NET
description: TextStyle propriété. Obtient ou définit ladresse du lien hypertexte. Doit être défini si la valeur deIsHyperlink la propriété est vraie.
type: docs
weight: 60
url: /fr/net/aspose.note/textstyle/hyperlinkaddress/
---
## TextStyle.HyperlinkAddress property

Obtient ou définit l'adresse du lien hypertexte. Doit être défini si la valeur de[`IsHyperlink`](../ishyperlink/) la propriété est vraie.

```csharp
public string HyperlinkAddress { get; set; }
```

### Exemples

Montre comment lier un lien hypertexte à un texte.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Tasks();

// Crée un objet de la classe Document
Document doc = new Document();

RichText titleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append("Title!");

Outline outline = new Outline()
                      {
                          MaxWidth = 200,
                          MaxHeight = 200,
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };

TextStyle textStyleRed = new TextStyle
                             {
                                 FontColor = Color.Red,
                                 FontName = "Arial",
                                 FontSize = 10,
                             };

TextStyle textStyleHyperlink = new TextStyle
                                   {
                                       IsHyperlink = true,
                                       HyperlinkAddress = "www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// Ajout d'éléments de contour
outline.AppendChildLast(outlineElem);

// Initialise l'objet de la classe Titre
Title title = new Title() { TitleText = titleText };

// Initialise l'objet de la classe Page
Page page = new Note.Page() { Title = title };

// Ajouter un noeud Contour
page.AppendChildLast(outline);

// Ajouter un nœud de page
doc.AppendChildLast(page);

// Enregistrer le document OneNote
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

### Voir également

* class [TextStyle](../)
* espace de noms [Aspose.Note](../../textstyle/)
* Assemblée [Aspose.Note](../../../)


