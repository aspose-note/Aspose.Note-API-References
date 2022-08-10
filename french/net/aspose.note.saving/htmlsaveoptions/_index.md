---
title: HtmlSaveOptions
second_title: Référence de l'API Aspose.Note pour .NET
description: Permet de spécifier des options supplémentaires lors de lenregistrement dun document au format HTML.
type: docs
weight: 680
url: /fr/net/aspose.note.saving/htmlsaveoptions/
---
## HtmlSaveOptions class

Permet de spécifier des options supplémentaires lors de l'enregistrement d'un document au format HTML.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions)() | Default_Constructor |

## Propriétés

| Nom | La description |
| --- | --- |
| [CssPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/cssperpagegeneration) { get; set; } | Obtient ou définit si le fichier StyleSheet sera généré séparément pour chaque nouvelle page. |
| [CssSavingCallback](../../aspose.note.saving/htmlsaveoptions/csssavingcallback) { get; set; } | Obtient ou définit le rappel appelé pour créer une ressource pour stocker CSS. |
| [DocumentPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/documentperpagegeneration) { get; set; } | Obtient ou définit une valeur indiquant si la génération de document par page est activée. |
| [ExportCss](../../aspose.note.saving/htmlsaveoptions/exportcss) { get; set; } | Obtient ou définit la manière dont le CSS est exporté. |
| [ExportFonts](../../aspose.note.saving/htmlsaveoptions/exportfonts) { get; set; } | Obtient ou définit la manière dont les polices sont exportées. |
| [ExportImages](../../aspose.note.saving/htmlsaveoptions/exportimages) { get; set; } | Obtient ou définit la façon dont les images sont exportées. |
| [FontFaceTypes](../../aspose.note.saving/htmlsaveoptions/fontfacetypes) { get; set; } | Obtient ou définit les types de polices. |
| [FontSavingCallback](../../aspose.note.saving/htmlsaveoptions/fontsavingcallback) { get; set; } | Obtient ou définit le rappel appelé pour créer une ressource pour stocker la police. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem) { get; set; } | Obtient ou définit les paramètres de police à utiliser lors de l'enregistrement |
| [ImageSavingCallback](../../aspose.note.saving/htmlsaveoptions/imagesavingcallback) { get; set; } | Obtient ou définit le rappel appelé pour créer une ressource pour stocker l'image. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount) { get; set; } | Obtient ou définit le nombre de pages à enregistrer. Par défaut estMaxValue ce qui signifie que toutes les pages du document seront rendues. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex) { get; set; } | Obtient ou définit l'index de la première page à enregistrer. Par défaut est 0. |
| [PageSavingCallback](../../aspose.note.saving/htmlsaveoptions/pagesavingcallback) { get; set; } | Obtient ou définit le rappel qui est appelé pour créer une ressource pour stocker la page. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat) { get; } | Obtient le format dans lequel le document est enregistré. |

### Exemples

Montre comment enregistrer un document au format html en stockant toutes les ressources (css/fonts/images) dans des fichiers séparés.

```csharp
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

var options = new HtmlSaveOptions()
             {
                 ExportCss = ResourceExportType.ExportAsStream,
                 ExportFonts = ResourceExportType.ExportAsStream,
                 ExportImages = ResourceExportType.ExportAsStream,
                 FontFaceTypes = FontFaceType.Ttf
             };
document.Save(dataDir + "document_out.html", options);
```

Montre comment enregistrer un document dans un flux au format html avec intégration de toutes les ressources (css/fonts/images).

```csharp
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

var options = new HtmlSaveOptions()
             {
                 ExportCss = ResourceExportType.ExportEmbedded,
                 ExportFonts = ResourceExportType.ExportEmbedded,
                 ExportImages = ResourceExportType.ExportEmbedded,
                 FontFaceTypes = FontFaceType.Ttf
             };

var r = new MemoryStream();
document.Save(r, options);
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

Montre comment enregistrer un document au format html en stockant toutes les ressources (css/fonts/images) en utilisant des rappels définis par l'utilisateur.

```csharp
// Le code ci-dessous crée le dossier 'documentFolder' contenant document.html, le dossier 'css' avec le fichier 'style.css', le dossier 'images' avec les images et le dossier 'fonts' avec les polices.
// Le fichier 'style.css' contiendra à la fin la chaîne suivante "/* Cette ligne est ajoutée pour être diffusée manuellement par l'utilisateur */"
var savingCallbacks = new UserSavingCallbacks()
                          {
                              RootFolder = "documentFolder",
                              CssFolder = "css",
                              KeepCssStreamOpened = true,
                              ImagesFolder = "images",
                              FontsFolder = "fonts"
                          };
var options = new HtmlSaveOptions
              {
                  FontFaceTypes = FontFaceType.Ttf,
                  CssSavingCallback = savingCallbacks,
                  FontSavingCallback = savingCallbacks,
                  ImageSavingCallback = savingCallbacks
              };

if (!Directory.Exists(savingCallbacks.RootFolder))
{
    Directory.CreateDirectory(savingCallbacks.RootFolder);
}

string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

using (var stream = File.Create(Path.Combine(savingCallbacks.RootFolder, "document.html")))
{
    document.Save(stream, options);
}

using (var writer = new StreamWriter(savingCallbacks.CssStream))
{
    writer.WriteLine();
    writer.WriteLine("/* This line is appended to stream manually by user */");
}
```

### Voir également

* class [SaveOptions](../saveoptions)
* espace de noms [Aspose.Note.Saving](../../aspose.note.saving)
* Assemblée [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
