---
title: Style.FontName
second_title: Référence de l'API Aspose.Note pour .NET
description: Style propriété. Obtient ou définit le nom de la police.
type: docs
weight: 20
url: /fr/net/aspose.note/style/fontname/
---
## Style.FontName property

Obtient ou définit le nom de la police.

```csharp
public string FontName { get; set; }
```

### Exemples

Manipulez par format de texte en utilisant le style de paragraphe.

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = new ParagraphStyle() { FontName = "Courier New", FontSize = 20 } }
                .Append($"DefaultParagraphFontAndSize{Environment.NewLine}")
                .Append($"OnlyDefaultParagraphFont{Environment.NewLine}", new TextStyle() { FontSize = 14 })
                .Append("OnlyDefaultParagraphFontSize", new TextStyle() { FontName = "Verdana" });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetDefaultParagraphStyle.one"));
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

* class [Style](../)
* espace de noms [Aspose.Note](../../style/)
* Assemblée [Aspose.Note](../../../)


