---
title: RichText
second_title: Référence de l'API Aspose.Note pour .NET
description: Représente un texte enrichi.
type: docs
weight: 510
url: /fr/net/aspose.note/richtext/
---
## RichText class

Représente un texte enrichi.

```csharp
public sealed class RichText : Node, IEnumerable<char>, IOutlineElementChildNode, ITaggable
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [RichText](richtext#constructor)() | Initialise une nouvelle instance du[`RichText`](../richtext) classe. |

## Propriétés

| Nom | La description |
| --- | --- |
| [Alignment](../../aspose.note/richtext/alignment) { get; set; } | Obtient ou définit l'alignement. |
| [Document](../../aspose.note/node/document) { get; } | Obtient le document du nœud. |
| virtual [IsComposite](../../aspose.note/node/iscomposite) { get; } | Obtient une valeur indiquant si ce nœud est composite. Si vrai, le nœud peut avoir des nœuds enfants. |
| [LastModifiedTime](../../aspose.note/richtext/lastmodifiedtime) { get; set; } | Obtient ou définit l'heure de la dernière modification. |
| [Length](../../aspose.note/richtext/length) { get; } | Obtient la longueur du texte. |
| [LineSpacing](../../aspose.note/richtext/linespacing) { get; set; } | Obtient ou définit l'interligne. |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | Obtient le nœud suivant au même niveau d'arborescence de nœuds. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | Obtient le type de nœud. |
| [ParagraphStyle](../../aspose.note/richtext/paragraphstyle) { get; set; } | Obtient ou définit le style de paragraphe. Ces paramètres sont utilisés s'il n'y a pas d'objet TextStyle correspondant dansStyles collection soit cet objet ne spécifie pas un paramètre nécessaire. |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | Obtient le nœud parent. |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | Obtient le nœud précédent au même niveau d'arborescence de nœuds. |
| [SpaceAfter](../../aspose.note/richtext/spaceafter) { get; set; } | Obtient ou définit la quantité minimale d'espace après. |
| [SpaceBefore](../../aspose.note/richtext/spacebefore) { get; set; } | Obtient ou définit la quantité minimale d'espace avant. |
| [Tags](../../aspose.note/richtext/tags) { get; } | Obtient la liste de toutes les balises d'un paragraphe. |
| [Text](../../aspose.note/richtext/text) { get; set; } | Obtient ou définit le texte. La chaîne NE DOIT PAS contenir de caractères de la valeur 10 (saut de ligne). |
| [TextRuns](../../aspose.note/richtext/textruns) { get; } | Obtient la collection d'exécutions de texte. |

## Méthodes

| Nom | La description |
| --- | --- |
| override [Accept](../../aspose.note/richtext/accept)(DocumentVisitor) | Accepte le visiteur du nœud. |
| [Append](../../aspose.note/richtext/append#append)(string) | Ajoute une chaîne à la dernière plage de texte. |
| [Append](../../aspose.note/richtext/append#append_1)(string, TextStyle) | Ajoute une chaîne à la fin. |
| [AppendFront](../../aspose.note/richtext/appendfront#appendfront)(string) | Ajoute une chaîne au début de la première plage de texte. |
| [AppendFront](../../aspose.note/richtext/appendfront#appendfront_1)(string, TextStyle) | Ajoute une chaîne devant. |
| [Clear](../../aspose.note/richtext/clear)() | Efface le contenu de cette instance. |
| [GetEnumerator](../../aspose.note/richtext/getenumerator)() | Renvoie un énumérateur qui parcourt les caractères de cet objet RichText. |
| [IndexOf](../../aspose.note/richtext/indexof#indexof)(char) | Renvoie l'index de base zéro de la première occurrence du caractère Unicode spécifié dans cette chaîne. |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_3)(string) | Renvoie l'index de base zéro de la première occurrence de la chaîne spécifiée dans cette instance. |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_1)(char, int) | Renvoie l'index de base zéro de la première occurrence du caractère Unicode spécifié dans cette chaîne. La recherche commence à une position de caractère spécifiée. |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_4)(string, int) | Renvoie l'index de base zéro de la première occurrence de la chaîne spécifiée dans cette instance. La recherche commence à une position de caractère spécifiée. |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_8)(string, StringComparison) | Renvoie l'index de base zéro de la première occurrence de la chaîne spécifiée dans l'instance actuelle. Un paramètre spécifie le type de recherche à utiliser pour la chaîne spécifiée. |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_2)(char, int, int) | Renvoie l'index de base zéro de la première occurrence du caractère spécifié dans cette instance. La recherche commence à une position de caractère spécifiée et examine un nombre spécifié de positions de caractère. |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_5)(string, int, int) | Renvoie l'index de base zéro de la première occurrence de la chaîne spécifiée dans cette instance. La recherche commence à une position de caractère spécifiée et examine un nombre spécifié de positions de caractère. |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_7)(string, int, StringComparison) | Renvoie l'index de base zéro de la première occurrence de la chaîne spécifiée dans l'instance actuelle. Les paramètres spécifient la position de recherche de départ dans la chaîne actuelle et le type de recherche à utiliser pour la chaîne spécifiée. |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_6)(string, int, int, StringComparison) | Renvoie l'index de base zéro de la première occurrence de la chaîne spécifiée dans l'instance actuelle. |
| [Insert](../../aspose.note/richtext/insert#insert)(int, string) | Insère une chaîne spécifiée à une position d'index spécifiée dans cette instance. |
| [Insert](../../aspose.note/richtext/insert#insert_1)(int, string, TextStyle) | Insère une chaîne spécifiée avec un style spécifié à une position d'index spécifiée dans cette instance. |
| [Remove](../../aspose.note/richtext/remove#remove)(int) | Supprime tous les caractères de l'instance actuelle, en commençant à une position spécifiée et en continuant jusqu'à la dernière position. |
| [Remove](../../aspose.note/richtext/remove#remove_1)(int, int) | Supprime le nombre spécifié de caractères dans l'instance actuelle en commençant à une position spécifiée. |
| [Replace](../../aspose.note/richtext/replace#replace)(char, char) | Remplace toutes les occurrences d'un caractère Unicode spécifié dans cette instance par un autre caractère Unicode spécifié. |
| [Replace](../../aspose.note/richtext/replace#replace_1)(string, string) | Remplace toutes les occurrences d'une chaîne spécifiée dans l'instance actuelle par une autre chaîne spécifiée. |
| [Replace](../../aspose.note/richtext/replace#replace_2)(string, string, TextStyle) | Remplace toutes les occurrences d'une chaîne spécifiée dans l'instance actuelle par une autre chaîne spécifiée dans le style spécifié. |
| [Trim](../../aspose.note/richtext/trim#trim)() | Supprime tous les espaces blancs de début et de fin. |
| [Trim](../../aspose.note/richtext/trim#trim_1)(char) | Supprime toutes les instances de début et de fin d'un caractère. |
| [Trim](../../aspose.note/richtext/trim#trim_2)(params char[]) | Supprime toutes les occurrences de début et de fin d'un ensemble de caractères spécifié dans un tableau. |
| [TrimEnd](../../aspose.note/richtext/trimend#trimend)() | Supprime tous les caractères d'espace blanc de fin. |
| [TrimEnd](../../aspose.note/richtext/trimend#trimend_1)(char) | Supprime toutes les occurrences de fin d'un caractère. |
| [TrimEnd](../../aspose.note/richtext/trimend#trimend_2)(params char[]) | Supprime toutes les occurrences de fin d'un ensemble de caractères spécifié dans un tableau. |
| [TrimStart](../../aspose.note/richtext/trimstart#trimstart)() | Supprime tous les premiers caractères d'espace blanc. |
| [TrimStart](../../aspose.note/richtext/trimstart#trimstart_1)(char) | Supprime toutes les occurrences principales d'un caractère spécifié. |
| [TrimStart](../../aspose.note/richtext/trimstart#trimstart_2)(params char[]) | Supprime toutes les occurrences principales d'un ensemble de caractères spécifié dans un tableau. |

### Exemples

Montre comment obtenir tout le texte du document.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Text();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Récupérer le texte
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// Affiche le texte sur l'écran de sortie
Console.WriteLine(text);
```

Montre comment obtenir tout le texte de la page.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Text();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Récupère la liste des nœuds de la page
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // Récupérer le texte
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // Affiche le texte sur l'écran de sortie
    Console.WriteLine(text);
}
```

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

Montre comment définir un titre pour une page.

```csharp
string dataDir = RunExamples.GetDataDir_Text();
string outputPath = dataDir + "CreateTitleMsStyle_out.one";

var doc = new Document();
var page = new Page(doc);

page.Title = new Title(doc)
{
    TitleText = new RichText(doc)
    {
        Text = "Title text.",
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleDate = new RichText(doc)
    {
        Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture),
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleTime = new RichText(doc)
    {
        Text = "12:34",
        ParagraphStyle = ParagraphStyle.Default
    }
};

doc.AppendChildLast(page);

doc.Save(outputPath);
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

Montre comment parcourir toutes les pages et effectuer un remplacement dans le texte.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Récupère tous les nœuds RichText
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Remplace le texte d'une forme
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

// Enregistrer dans n'importe quel format de fichier pris en charge
oneFile.Save(dataDir, SaveFormat.Pdf);
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

Montre comment parcourir le texte de la page et effectuer un remplacement.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// Récupère tous les nœuds RichText
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Remplace le texte d'une forme
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// Enregistrer dans n'importe quel format de fichier pris en charge
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Montre comment créer un document et l'enregistrer au format html à l'aide des options par défaut.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initialiser le document OneNote
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

// Style par défaut pour tout le texte du document.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// Enregistrer au format HTML
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

Montre comment ajouter un nouveau paragraphe avec une balise.

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
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
RichText text = new RichText(doc) { Text = "OneNote text.", ParagraphStyle = textStyle };
text.Tags.Add(NoteTag.CreateYellowStar());

// Ajouter un nœud de texte
outlineElem.AppendChildLast(text);

// Ajoute un nœud d'élément de contour
outline.AppendChildLast(outlineElem);

// Ajoute un nœud de contour
page.AppendChildLast(outline);

// Ajouter un nœud de page
doc.AppendChildLast(page);

// Enregistrer le document OneNote
dataDir = dataDir + "AddTextNodeWithTag_out.one";
doc.Save(dataDir);
```

Montre comment créer un document et enregistrer au format html une plage de pages spécifiée.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initialiser le document OneNote
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Style par défaut pour tout le texte du document.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// Enregistrer au format HTML
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

Montre comment accéder aux détails d'une balise.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Tags();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "TagFile.one");

// Récupère tous les nœuds RichText
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Itérer à travers chaque nœud
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // Récupérer les propriétés
            Console.WriteLine($"    Completed Time: {noteTag.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTag.CreationTime}");
            Console.WriteLine($"    Font Color: {noteTag.FontColor}");
            Console.WriteLine($"    Status: {noteTag.Status}");
            Console.WriteLine($"    Label: {noteTag.Label}");
            Console.WriteLine($"    Icon: {noteTag.Icon}");
            Console.WriteLine($"    High Light: {noteTag.Highlight}");
        }
    }
}
```

Montre comment créer un document avec un texte.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Crée un objet de la classe Document
Document doc = new Document();

// Initialise l'objet de la classe Page
Page page = new Page(doc);

// Initialise l'objet de la classe Outline
Outline outline = new Outline(doc);

// Initialise l'objet de classe OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Initialise l'objet de classe TextStyle et définit les propriétés de formatage
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Initialise l'objet de classe RichText et applique le style de texte
RichText text = new RichText(doc) { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// Ajouter un noeud RichText
outlineElem.AppendChildLast(text);

// Ajoute le noeud OutlineElement
outline.AppendChildLast(outlineElem);

// Ajouter un noeud Contour
page.AppendChildLast(outline);

// Ajouter un nœud de page
doc.AppendChildLast(page);

// Enregistrer le document OneNote
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
doc.Save(dataDir);
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

Montre comment préparer un modèle pour une réunion hebdomadaire.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Tags();

// Crée un objet de la classe Document
var headerStyle = new ParagraphStyle() { FontName = "Calibri", FontSize = 16 };
var bodyStyle = new ParagraphStyle() { FontName = "Calibri", FontSize = 12 };

var d = new Document();
bool restartFlag = true;
var outline = d.AppendChildLast(new Page()
                                    {
                                        Title = new Title() { TitleText = new RichText() { Text = $"Weekly meeting {DateTime.Today:d}", ParagraphStyle = ParagraphStyle.Default } }
                                    })
               .AppendChildLast(new Outline() { VerticalOffset = 30, HorizontalOffset = 30 });

outline.AppendChildLast(new OutlineElement())
       .AppendChildLast(new RichText() { Text = "Important", ParagraphStyle = headerStyle });
foreach (var e in new[] { "First", "Second", "Third" })
{
    outline.AppendChildLast(new OutlineElement() { NumberList = CreateListNumberingStyle(bodyStyle, restartFlag) })
           .AppendChildLast(new RichText() { Text = e, ParagraphStyle = bodyStyle });
    restartFlag = false;
}

outline.AppendChildLast(new OutlineElement())
       .AppendChildLast(new RichText() { Text = "TO DO", ParagraphStyle = headerStyle, SpaceBefore = 15 });
restartFlag = true;
foreach (var e in new[] { "First", "Second", "Third" })
{
    outline.AppendChildLast(new OutlineElement() { NumberList = CreateListNumberingStyle(bodyStyle, restartFlag) })
           .AppendChildLast(new RichText() { Text = e, ParagraphStyle = bodyStyle, Tags = { NoteCheckBox.CreateBlueCheckBox() } });
    restartFlag = false;
}

d.Save(Path.Combine(dataDir, "meetingNotes.one"));
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

* class [Node](../node)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode)
* interface [ITaggable](../itaggable)
* espace de noms [Aspose.Note](../../aspose.note)
* Assemblée [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
