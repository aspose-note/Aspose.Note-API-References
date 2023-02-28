---
title: Title.TitleText
second_title: Référence de l'API Aspose.Note pour .NET
description: Title propriété. Obtient ou définit le texte du titre.
type: docs
weight: 60
url: /fr/net/aspose.note/title/titletext/
---
## Title.TitleText property

Obtient ou définit le texte du titre.

```csharp
public RichText TitleText { get; set; }
```

### Exemples

Montre comment modifier l'historique de la page.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Pages();

// Charger le document OneNote et obtenir le premier enfant           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.RemoveRange(0, 1);

pageHistory[0] = new Page(document);
if (pageHistory.Count > 1)
{
    pageHistory[1].Title.TitleText.Text = "New Title";

    pageHistory.Add(new Page(document));

    pageHistory.Insert(1, new Page(document));

    document.Save(dataDir + "ModifyPageHistory_out.one");
}
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

Montre comment créer un document avec une page de titre.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Crée un objet de la classe Document
Document doc = new Aspose.Note.Document();

// Initialise l'objet de la classe Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Style par défaut pour tout le texte du document.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Définir les propriétés du titre de la page
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Ajoute le noeud Page dans le document
doc.AppendChildLast(page);

// Enregistrer le document OneNote
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

Montre comment enregistrer un document dans différents formats.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initialise le nouveau Document
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// Initialise la nouvelle Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Style par défaut pour tout le texte du document.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Ajoute le nœud de la page
doc.AppendChildLast(page);

// Enregistrez le document OneNote dans différents formats, définissez la taille de la police du texte et détectez manuellement les modifications de mise en page.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

### Voir également

* class [RichText](../../richtext/)
* class [Title](../)
* espace de noms [Aspose.Note](../../title/)
* Assemblée [Aspose.Note](../../../)


