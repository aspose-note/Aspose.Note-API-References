---
title: PageIndex
second_title: Référence de l'API Aspose.Note pour .NET
description: Obtient ou définit lindex de la première page à enregistrer. Par défaut est 0.
type: docs
weight: 30
url: /fr/net/aspose.note.saving/saveoptions/pageindex/
---
## SaveOptions.PageIndex property

Obtient ou définit l'index de la première page à enregistrer. Par défaut est 0.

```csharp
public int PageIndex { get; set; }
```

### Exemples

Montre comment enregistrer un document au format png.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initialise l'objet ImageSaveOptions 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // Définir l'index de la page
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// Enregistrez le document au format PNG.
oneFile.Save(dataDir, opts);
```

Montre comment enregistrer un document au format pdf.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initialise l'objet PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Définit l'index de la première page à enregistrer
                              PageIndex = 0,

                              // Définir le nombre de pages
                              PageCount = 1,
                          };

// Enregistrer le document au format PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Montre comment enregistrer un document au format pdf en utilisant des paramètres spécifiques.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Initialise l'objet PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Utiliser la compression Jpeg
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Qualité pour la compression JPEG
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
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

Montre comment créer un document avec du texte enrichi formaté.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Crée un objet de la classe Document
Document doc = new Document();

// Initialise l'objet de la classe Page
Page page = new Page();

// Initialise l'objet de la classe Titre
Title title = new Title();

// Initialise l'objet de classe TextStyle et définit les propriétés de formatage
ParagraphStyle defaultTextStyle = new ParagraphStyle
                                      {
                                          FontColor = Color.Black,
                                          FontName = "Arial",
                                          FontSize = 10
                                      };

RichText titleText = new RichText() { ParagraphStyle = defaultTextStyle }.Append("Title!");
Outline outline = new Outline()
                      {
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };
OutlineElement outlineElem = new OutlineElement();

TextStyle textStyleForHelloWord = new TextStyle
                                      {
                                          FontColor = Color.Red,
                                          FontName = "Arial",
                                          FontSize = 10,
                                      };

TextStyle textStyleForOneNoteWord = new TextStyle
                                        {
                                            FontColor = Color.Green,
                                            FontName = "Calibri",
                                            FontSize = 10,
                                            IsItalic = true,
                                        };

TextStyle textStyleForTextWord = new TextStyle
                                     {
                                         FontColor = Color.Blue,
                                         FontName = "Arial",
                                         FontSize = 15,
                                         IsBold = true,
                                         IsItalic = true,
                                     };

RichText text = new RichText() { ParagraphStyle = defaultTextStyle }
                    .Append("Hello", textStyleForHelloWord)
                    .Append(" OneNote", textStyleForOneNoteWord)
                    .Append(" text", textStyleForTextWord)
                    .Append("!", TextStyle.Default);

title.TitleText = titleText;

// Définir le titre de la page
page.Title = title;

// Ajouter un noeud RichText
outlineElem.AppendChildLast(text);

// Ajoute le noeud OutlineElement
outline.AppendChildLast(outlineElem);

// Ajouter un noeud Contour
page.AppendChildLast(outline);

// Ajouter un nœud de page
doc.AppendChildLast(page);

// Enregistrer le document OneNote
dataDir = dataDir + "CreateDocWithFormattedRichText_out.one";
doc.Save(dataDir);
```

### Voir également

* class [SaveOptions](../../saveoptions)
* espace de noms [Aspose.Note.Saving](../../saveoptions)
* Assemblée [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
