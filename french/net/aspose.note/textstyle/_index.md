---
title: Class TextStyle
second_title: Référence de l'API Aspose.Note pour .NET
description: Aspose.Note.TextStyle classe. Spécifie le style de texte.
type: docs
weight: 970
url: /fr/net/aspose.note/textstyle/
---
## TextStyle class

Spécifie le style de texte.

```csharp
public sealed class TextStyle : Style
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [TextStyle](textstyle/)() | Default_Constructor |

## Propriétés

| Nom | La description |
| --- | --- |
| static [Default](../../aspose.note/textstyle/default/) { get; } | Obtient le style avec la culture "en-US". |
| static [DefaultMsOneNoteTitleDateStyle](../../aspose.note/textstyle/defaultmsonenotetitledatestyle/) { get; } | Obtient le style par défaut pour la date du titre dans MS OneNote. |
| static [DefaultMsOneNoteTitleTextStyle](../../aspose.note/textstyle/defaultmsonenotetitletextstyle/) { get; } | Obtient le style par défaut pour le texte du titre dans MS OneNote. |
| static [DefaultMsOneNoteTitleTimeStyle](../../aspose.note/textstyle/defaultmsonenotetitletimestyle/) { get; } | Obtient le style par défaut pour l'heure du titre dans MS OneNote. |
| [FontColor](../../aspose.note/style/fontcolor/) { get; set; } | Obtient ou définit la couleur de la police. |
| [FontName](../../aspose.note/style/fontname/) { get; set; } | Obtient ou définit le nom de la police. |
| [FontSize](../../aspose.note/style/fontsize/) { get; set; } | Obtient ou définit la taille de la police. |
| [FontStyle](../../aspose.note/style/fontstyle/) { get; } | Obtient le style de police. |
| [Highlight](../../aspose.note/style/highlight/) { get; set; } | Obtient ou définit la couleur de surbrillance. |
| [HyperlinkAddress](../../aspose.note/textstyle/hyperlinkaddress/) { get; set; } | Obtient ou définit l'adresse du lien hypertexte. Doit être défini si la valeur de[`IsHyperlink`](./ishyperlink/) la propriété est vraie. |
| [IsBold](../../aspose.note/style/isbold/) { get; set; } | Obtient ou définit une valeur indiquant si le style de texte est en gras. |
| [IsHidden](../../aspose.note/textstyle/ishidden/) { get; set; } | Obtient ou définit une valeur indiquant si le style de texte est masqué. |
| [IsHyperlink](../../aspose.note/textstyle/ishyperlink/) { get; set; } | Obtient ou définit une valeur indiquant si le style de texte est un lien hypertexte. |
| [IsItalic](../../aspose.note/style/isitalic/) { get; set; } | Obtient ou définit une valeur indiquant si le style de texte est en italique. |
| [IsMathFormatting](../../aspose.note/textstyle/ismathformatting/) { get; set; } | Obtient ou définit une valeur indiquant si le style de texte est au format mathématique. |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough/) { get; set; } | Obtient ou définit une valeur indiquant si le style de texte est barré. |
| [IsSubscript](../../aspose.note/style/issubscript/) { get; set; } | Obtient ou définit une valeur indiquant si le style de texte est en indice. |
| [IsSuperscript](../../aspose.note/style/issuperscript/) { get; set; } | Obtient ou définit une valeur indiquant si le style de texte est en exposant. |
| [IsUnderline](../../aspose.note/style/isunderline/) { get; set; } | Obtient ou définit une valeur indiquant si le style de texte est souligné. |
| [Language](../../aspose.note/textstyle/language/) { get; set; } | Obtient ou définit la langue du texte. |

## Méthodes

| Nom | La description |
| --- | --- |
| override [Equals](../../aspose.note/textstyle/equals/#equals_1)(object) | Détermine si l'objet spécifié est égal à l'objet actuel. |
| [Equals](../../aspose.note/textstyle/equals/#equals)(TextStyle) | Détermine si l'objet spécifié est égal à l'objet actuel. |
| override [GetHashCode](../../aspose.note/textstyle/gethashcode/)() | Sert de fonction de hachage pour le type. |

### Exemples

Mettons l'accent sur les titres de page parmi les autres en-têtes en augmentant la taille de la police.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Charge le document dans Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Parcourt les titres de la page.
foreach (var title in document.Select(e => e.Title.TitleText))
{
    title.ParagraphStyle.FontSize = 24;
    title.ParagraphStyle.IsBold = true;

    foreach (var run in title.TextRuns)
    {
        run.Style.FontSize = 24;
        run.Style.IsBold = true;
    }
}

document.Save(Path.Combine(dataDir, "ChangePageTitleStyle.pdf"));
```

Soulignons les dernières modifications du texte en les mettant en surbrillance.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Charge le document dans Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Récupère les nœuds RichText modifiés la semaine dernière.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // Définir la couleur de surbrillance
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // Définir la couleur de surbrillance
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

Définir la langue de vérification d'un texte.

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = ParagraphStyle.Default };
text.Append("United States", new TextStyle() { Language = CultureInfo.GetCultureInfo("en-US") })
    .Append(" Germany", new TextStyle() { Language = CultureInfo.GetCultureInfo("de-DE") })
    .Append(" China", new TextStyle() { Language = CultureInfo.GetCultureInfo("zh-CN") });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetProofingLanguageForText.one"));
```

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

* class [Style](../style/)
* espace de noms [Aspose.Note](../../aspose.note/)
* Assemblée [Aspose.Note](../../)


